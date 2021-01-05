---
title: Järjestelmänvalvojien lisääminen ja hallinta
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7424"
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755436"
---
# <a name="how-to-add-and-manage-admins"></a><span data-ttu-id="605f6-102">Järjestelmänvalvojien lisääminen ja hallinta</span><span class="sxs-lookup"><span data-stu-id="605f6-102">How to add and manage admins</span></span>

<span data-ttu-id="605f6-103">Ongelman kuva uksen perusteella olemme löytäneet ratkaisun.</span><span class="sxs-lookup"><span data-stu-id="605f6-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="605f6-104">Useimmat Asiakkaat pystyivät ratkaisemaan ongelmaansa sen jälkeen, kun he ovat seuraavat asia kirjojamme.</span><span class="sxs-lookup"><span data-stu-id="605f6-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="605f6-105">Jos haluat hallita Microsoft-asiakas sopimusta (MCA), voit käyttää eri rooleja, joilla on haluttu käyttö oikeus taso.</span><span class="sxs-lookup"><span data-stu-id="605f6-105">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="605f6-106">Nämä roolit ovat niiden sisäisten Azure-palvelu roolien lisäksi, joiden avulla voit hallita resurssejasi.</span><span class="sxs-lookup"><span data-stu-id="605f6-106">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="605f6-107">**Voit lisätä laskutus rooleja Azure-portaalissa seuraavasti:**</span><span class="sxs-lookup"><span data-stu-id="605f6-107">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="605f6-108">Kirjaudu sisään Azure- [portaaliin](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="605f6-108">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="605f6-109">Hae *kustannusten hallinta + laskutus*.</span><span class="sxs-lookup"><span data-stu-id="605f6-109">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="605f6-110">Valitse käytön hallinta (IAM) sellaisen käyttö alueen mukaan, kuten laskutus tili, laskutus profiili tai laskun osa, jossa haluat myöntää käyttö oikeuden.</span><span class="sxs-lookup"><span data-stu-id="605f6-110">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="605f6-111">Käyttö oikeuksien hallinta-sivulla on lueteltu käyttäjät ja ryhmät, jotka on määritetty kullekin roolille kyseiselle alueelle.</span><span class="sxs-lookup"><span data-stu-id="605f6-111">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="605f6-112">Jos haluat antaa käyttäjälle käyttö oikeuden, valitse **Lisää** sivun yläreunasta.</span><span class="sxs-lookup"><span data-stu-id="605f6-112">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="605f6-113">Valitse rooli avattavasta *rooli* -luettelosta.</span><span class="sxs-lookup"><span data-stu-id="605f6-113">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="605f6-114">Kirjoita sen käyttäjän Sähkö posti osoite, jolle haluat myöntää käyttö oikeuden.</span><span class="sxs-lookup"><span data-stu-id="605f6-114">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="605f6-115">Määritä rooli valitsemalla **Tallenna** .</span><span class="sxs-lookup"><span data-stu-id="605f6-115">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="605f6-116">Jos haluat poistaa käyttäjän käyttö oikeuden, valitse käyttäjä, jonka rooli määritystä haluat poistaa.</span><span class="sxs-lookup"><span data-stu-id="605f6-116">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="605f6-117">Valitse **Poista**.</span><span class="sxs-lookup"><span data-stu-id="605f6-117">Select **Remove**.</span></span>

<span data-ttu-id="605f6-118">**Suositellut asiakirjat**</span><span class="sxs-lookup"><span data-stu-id="605f6-118">**Recommended Documents**</span></span>

- [<span data-ttu-id="605f6-119">Laskutus rooli määritykset</span><span class="sxs-lookup"><span data-stu-id="605f6-119">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="605f6-120">Laskutus tilin roolit ja tehtävät</span><span class="sxs-lookup"><span data-stu-id="605f6-120">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="605f6-121">MCA-laskutus tilin käytön aloittaminen</span><span class="sxs-lookup"><span data-stu-id="605f6-121">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="605f6-122">Microsoft-asiakas sopimuksen käytön tarkistaminen</span><span class="sxs-lookup"><span data-stu-id="605f6-122">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
