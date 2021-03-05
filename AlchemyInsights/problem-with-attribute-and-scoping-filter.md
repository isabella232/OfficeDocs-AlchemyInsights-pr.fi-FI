---
title: Määritettä ja suodatusta koskevat ongelmat
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481365"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="bf349-102">Määritettä ja suodatusta koskevat ongelmat</span><span class="sxs-lookup"><span data-stu-id="bf349-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="bf349-103">**Ongelma ristiriitaisten UPN-arvojen kanssa**</span><span class="sxs-lookup"><span data-stu-id="bf349-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="bf349-104">Workday to AD User Provisioning Workday to AD User Provisioning (Työpäivä) näyttää **virhesanoman HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique.**</span><span class="sxs-lookup"><span data-stu-id="bf349-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="bf349-105">Toiminto epäonnistui, koska lisäykselle tai muokkaukselle annettu UPN-arvo ei ole yksilöllinen koko metsää.</span><span class="sxs-lookup"><span data-stu-id="bf349-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="bf349-106">Virheen tiedot: **CONSTRAINT_ATT_TYPE - userPrincipalName.**</span><span class="sxs-lookup"><span data-stu-id="bf349-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="bf349-107">**UserPrincipalName-arvo,** jonka Työpäivä-yhdistin yrittää määrittää luodessaan AD-käyttäjätiliä, on jo ad-kohdetoimialueella.</span><span class="sxs-lookup"><span data-stu-id="bf349-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="bf349-108">Tämä tarkoittaa, että joko (1) käyttäjä on jo olemassa ja käyttäjän vastaava tunnuksen tarkistus epäonnistui, tai (2) UPN-luontisääntö loi ristiriitaisen arvon.</span><span class="sxs-lookup"><span data-stu-id="bf349-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="bf349-109">Seuraavassa on ehdotettuja ratkaisuvaiheita:</span><span class="sxs-lookup"><span data-stu-id="bf349-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="bf349-110">Jos käyttäjä on jo olemassa ja vastaavan tunnuksen tarkistus ei onnistunut yhdistämaan Työpäivä-tiliä Active Directory -tiliin, tarkista, onko vastaavan tunnusmääritteen (yleensä **työntekijätunnus)** sekä Työpäivä- että AD-tunnuksella tarkka vastine.</span><span class="sxs-lookup"><span data-stu-id="bf349-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="bf349-111">Jos heillä ei ole vastaavuustietoja, ne on korjattava.</span><span class="sxs-lookup"><span data-stu-id="bf349-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="bf349-112">Jos esimerkiksi Työpäivä-kohdan Työntekijätunnus on 001052 ja AD-arvo on 1052, valmistelumoduuli ei linkitä kahta tiliä ja yrittää luoda jo olemassa olevan käyttäjän.</span><span class="sxs-lookup"><span data-stu-id="bf349-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="bf349-113">Tässä tapauksessa voit muuttaa TYÖNTEKIJÄNTUNNUS-arvoa AD:ssä niin, että siihen sisällytetään etunollat, jotta siitä tulee 001052. </span><span class="sxs-lookup"><span data-stu-id="bf349-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="bf349-114">Jos UPN-luomislauseke ei luo yksilöllistä arvoa, harkitse kopiointia poistamisfunktion **SelectUniqueValue** avulla yksilöllistä arvoa joka kerta.</span><span class="sxs-lookup"><span data-stu-id="bf349-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="bf349-115">**Työpäiväksi AD-käyttäjien valmistelu ei määritä hallinnoijan määritearvoa AD-käyttäjätilille**</span><span class="sxs-lookup"><span data-stu-id="bf349-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="bf349-116">Työpäivä-asetukseksi AD-käyttäjien valmistelutyö ei määritä **ESIMIEHEN** määritearvoa AD-käyttäjätileille.</span><span class="sxs-lookup"><span data-stu-id="bf349-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="bf349-117">Kun tämä tapahtuu, on kaksi mahdollista skenaariota:</span><span class="sxs-lookup"><span data-stu-id="bf349-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="bf349-118">Työpäivä-päällikköä ei voi ratkaista vastaavaksi AD-käyttäjätiliksi, koska esimies ei ole laajuudessa.</span><span class="sxs-lookup"><span data-stu-id="bf349-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="bf349-119">Usean **AD-toimialueen** skenaariossa Työpäivä-päällikkö ei ole samassa toimialueessa kuin käyttäjä.</span><span class="sxs-lookup"><span data-stu-id="bf349-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="bf349-120">Yritä ratkaista ongelma seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="bf349-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="bf349-121">Jos olet määrittänyt vaikutusalueen suodattimia, tarkista ensin, onko esimies laajuudessa ja että se täyttää vaikutusalueen lausekkeen.</span><span class="sxs-lookup"><span data-stu-id="bf349-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="bf349-122">Jos esimies ei täytä vaikutusalueen suodatusta, muuta suodatinta niin, että myös esimies kuuluu valmistelutoiminnon piiriin.</span><span class="sxs-lookup"><span data-stu-id="bf349-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="bf349-123">Jos sinulla on useita AD-toimialueita, yhdistimellä on tunnettu rajoitus, joka rajoittaa toimialueidenvälisten hallintaviittausten ratkaisemista.</span><span class="sxs-lookup"><span data-stu-id="bf349-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="bf349-124">Lisätietoja työpäivän määrittämisestä automaattista valmistelua varten on opetusohjelmassa: Työpäivän määrittäminen [automaattista käyttäjien valmistelua varten.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="bf349-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













