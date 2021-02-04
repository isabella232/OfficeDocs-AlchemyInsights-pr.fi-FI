---
title: Ota käyttöön salasanan takaisinkirjoitus Azure AD Connectissa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 1e90aedab20c8abaa021ed980e868cea0503b7b1
ms.sourcegitcommit: db95fd628c45d9810e5af5c5a4e6388c793339ac
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093352"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="ecde2-102">Ota käyttöön salasanan takaisinkirjoitus Azure AD Connectissa</span><span class="sxs-lookup"><span data-stu-id="ecde2-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="ecde2-103">Jotta voit ottaa käyttöön salasanan palauttaminen takaisinkirjoituksen itsepalveluna, ota ensin käyttöön takaisinkirjoitusasetus Azure AD Connectissa.</span><span class="sxs-lookup"><span data-stu-id="ecde2-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="ecde2-104">Suorita seuraavat vaiheet Azure AD Connect -palvelimelta:</span><span class="sxs-lookup"><span data-stu-id="ecde2-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="ecde2-105">Kirjaudu sisään Azure AD Connect -palvelimelle ja käynnistä **Azure AD Connectin** ohjattu määritys.</span><span class="sxs-lookup"><span data-stu-id="ecde2-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="ecde2-106">Klikkaa **Tervetuloa**-sivulla **Määritä**.</span><span class="sxs-lookup"><span data-stu-id="ecde2-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="ecde2-107">Valitse **Lisätehtävät**-sivulta **Mukauta synkronointivaihtoehtoja** ja klikkaa sitten **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="ecde2-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="ecde2-108">Lisää **Yhdistä Azure AD:hen** -sivulla yleisen Azure-vuokraajan järjestelmänvalvojan kirjautumistiedot ja klikkaa **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="ecde2-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="ecde2-109">Klikkaa **Yhdistä hakemistot**- ja **Toimialue/OU** -suodatussivuilta **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="ecde2-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="ecde2-110">Valitse **Valinnaiset ominaisuudet** -sivulla valintaruutu kohdasta **Salasanan takaisinkirjoitus** ja klikkaa **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="ecde2-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="ecde2-111">Klikkaa **Valmis määritettäväksi** -sivulta **Määritä** ja odota, että prosessi suoritetaan loppuun.</span><span class="sxs-lookup"><span data-stu-id="ecde2-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="ecde2-112">Kun määritys on suoritettu loppuun, klikkaa **Lopeta**.</span><span class="sxs-lookup"><span data-stu-id="ecde2-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="ecde2-113">Kun salasanan takaisinkirjoitus on otettu käyttöön Azure AD Connectissa, määritä Azure AD SSPR takaisinkirjoitusta varten.</span><span class="sxs-lookup"><span data-stu-id="ecde2-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="ecde2-114">Ota käyttöön salasanan takaisinkirjoitus SSPR:ssä suorittamalla seuraavat vaiheet:</span><span class="sxs-lookup"><span data-stu-id="ecde2-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="ecde2-115">Kirjaudu Azure-portaaliin yleisen järjestelmänvalvojan tilillä.</span><span class="sxs-lookup"><span data-stu-id="ecde2-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="ecde2-116">Etsi ja valitse **Azure Active Directory**, klikkaa **Salasanan palauttaminen** ja klikkaa sitten **Paikallinen integrointi**.</span><span class="sxs-lookup"><span data-stu-id="ecde2-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="ecde2-117">Valitse **Kirjoitetaanko salasanat takaisin paikalliseen hakemistoon?** -kohdasta **Kyllä**.</span><span class="sxs-lookup"><span data-stu-id="ecde2-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="ecde2-118">Valitse **Sallitaanko käyttäjien poistaa tilien lukituksen palauttamatta salasanojaan?** -kohdasta **Kyllä**.</span><span class="sxs-lookup"><span data-stu-id="ecde2-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="ecde2-119">Kun olet valmis, valitse **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="ecde2-119">When ready, click **Save**.</span></span>

<span data-ttu-id="ecde2-120">Lue lisää artikkelista [Azure Active Directoryn salasanan palauttamisen takaisinkirjoitus itsepalveluna paikalliseen ympäristöön](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="ecde2-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="ecde2-121">Kun järjestelmänvalvoja palauttaa käyttäjän salasanan Azure-portaalissa, jos käyttäjä on organisaation ulkopuolinen tai salasanan hajautus on synkronoitu, salasana kirjoitetaan takaisin paikallisesti.</span><span class="sxs-lookup"><span data-stu-id="ecde2-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="ecde2-122">Tämä toiminto edellyttää Azure Premium -käyttöoikeutta (P1 tai P2), eikä sitä tällä hetkellä tueta Office-hallintaportaalissa.</span><span class="sxs-lookup"><span data-stu-id="ecde2-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
