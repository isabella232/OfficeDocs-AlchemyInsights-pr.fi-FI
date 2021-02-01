---
title: Tunnistetietoihin liittyvät ongelmat
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063628"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="3b6b7-102">Tunnistetietoihin liittyvät ongelmat</span><span class="sxs-lookup"><span data-stu-id="3b6b7-102">Issues with credentials</span></span>

<span data-ttu-id="3b6b7-103">[Microsoftin tunnistetietoympäristössä ja OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) -asiakastietojen työnkulussa kuvataan, miten ohjelma voidaan ohjelmoida suoraan OAuth 2.0 -asiakastietojen grant flow -tunnuksen avulla.</span><span class="sxs-lookup"><span data-stu-id="3b6b7-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="3b6b7-104">**Miten hallitsen sovelluksen salasanaa tai varmenteen tunnistetietoja?**</span><span class="sxs-lookup"><span data-stu-id="3b6b7-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="3b6b7-105">Azure CLI:ssä voit [käyttää az ad -sovelluksen](https://docs.microsoft.com/cli/azure/ad/app/credential) tunnistetietoja sovelluksen salasanan tai varmenteen tunnistetietojen poistamiseen, luetteloon tai palauttamiseen.</span><span class="sxs-lookup"><span data-stu-id="3b6b7-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="3b6b7-106">**Miten käyttäjät palauttavat salasanansa?**</span><span class="sxs-lookup"><span data-stu-id="3b6b7-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="3b6b7-107">Käyttäjien on [rekisteröitävä omatoiminen salasanan vaihto,](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) ennen kuin he voivat vaihtaa salasanansa.</span><span class="sxs-lookup"><span data-stu-id="3b6b7-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="3b6b7-108">Kun käyttäjä on rekisteröitynyt, hän voi palauttaa salasanansa noudattamalla tämän artikkelin ohjeita: Vaihda [työ- tai koulusalasanasi.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)</span><span class="sxs-lookup"><span data-stu-id="3b6b7-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="3b6b7-109">**Miten käyttäjät vaihtavat salasanansa?**</span><span class="sxs-lookup"><span data-stu-id="3b6b7-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="3b6b7-110">Käyttäjät voivat vaihtaa salasanansa noudattamalla tässä artikkelissa annettuja ohjeita: [Salasanan vaihtaminen.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)</span><span class="sxs-lookup"><span data-stu-id="3b6b7-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="3b6b7-111">He voivat myös [hallita sovelluksen salasanoja kaksivaiheista vahvistusta varten.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)</span><span class="sxs-lookup"><span data-stu-id="3b6b7-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="3b6b7-112">**Käyttäjäni saa virheilmoituksen, kun salasanaa muutetaan tai palautetaan**</span><span class="sxs-lookup"><span data-stu-id="3b6b7-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="3b6b7-113">Tämä linkki antaa tietoja yleisistä ongelmista, joita voi ilmetä, kun käyttäjä yrittää vaihtaa salasanansa: yleisiä [ongelmia ja heidän ratkaisujaan](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="3b6b7-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="3b6b7-114">**Minulla on ongelmia käyttäjän salasanan palauttamisessa**</span><span class="sxs-lookup"><span data-stu-id="3b6b7-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="3b6b7-115">Varmista, että sinulla on oikeus vaihtaa salasanoja.</span><span class="sxs-lookup"><span data-stu-id="3b6b7-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="3b6b7-116">*Vain yleiset järjestelmänvalvojat, salasanat ja käyttäjien järjestelmänvalvojat voivat vaihtaa käyttäjien salasanat.*</span><span class="sxs-lookup"><span data-stu-id="3b6b7-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="3b6b7-117">Yleiset järjestelmänvalvojat voivat myös palauttaa muiden järjestelmänvalvojan salasanat.</span><span class="sxs-lookup"><span data-stu-id="3b6b7-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="3b6b7-118">Varmista, että ymmärrät käyttöoikeusvaatimukset:</span><span class="sxs-lookup"><span data-stu-id="3b6b7-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="3b6b7-119">Sinulla on oltava vähintään yksi käyttöoikeus määritettynä organisaatiossasi:</span><span class="sxs-lookup"><span data-stu-id="3b6b7-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="3b6b7-120">**Vain pilvipalvelun käyttäjät** – mikä tahansa Office 365 (O365) maksettu SKU tai Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="3b6b7-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="3b6b7-121">**Pilvi- ja/tai paikalliskäyttäjät** – Azure AD Premium P1 tai P2, Enterprise Mobility + Security (EMS) tai Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="3b6b7-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="3b6b7-122">Lisätietoja käyttöoikeusvaatimuksista on kohdassa [Azure AD:n omatoimista salasanan vaihtoa koskevat käyttöoikeusvaatimukset.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="3b6b7-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="3b6b7-123">Jos haluat vaihtaa käyttäjän salasanan, etsi käyttäjä Azure AD:ssä.</span><span class="sxs-lookup"><span data-stu-id="3b6b7-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="3b6b7-124">Napsauta sitten käyttäjän yleiskatsausterässä Palauta salasana -painiketta.</span><span class="sxs-lookup"><span data-stu-id="3b6b7-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="3b6b7-125">**Salasanan vaihtopainike näkyy harmaana**</span><span class="sxs-lookup"><span data-stu-id="3b6b7-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="3b6b7-126">Sinulla ei ole oikeutta **palauttaa** tämän käyttäjän salasanoja.</span><span class="sxs-lookup"><span data-stu-id="3b6b7-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="3b6b7-127">*Vain yleiset järjestelmänvalvojat, salasanat ja käyttäjien järjestelmänvalvojat voivat vaihtaa käyttäjien salasanat.*</span><span class="sxs-lookup"><span data-stu-id="3b6b7-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="3b6b7-128">Yleiset järjestelmänvalvojat voivat myös palauttaa muiden järjestelmänvalvojan salasanat.</span><span class="sxs-lookup"><span data-stu-id="3b6b7-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="3b6b7-129">**Salasanan vaihto-osaa ei ole**</span><span class="sxs-lookup"><span data-stu-id="3b6b7-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="3b6b7-130">Sinulla ei ole oikeutta vaihtaa salasanoja.</span><span class="sxs-lookup"><span data-stu-id="3b6b7-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="3b6b7-131">*Vain yleiset järjestelmänvalvojat, salasanat ja käyttäjien järjestelmänvalvojat voivat vaihtaa käyttäjien salasanat.*</span><span class="sxs-lookup"><span data-stu-id="3b6b7-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="3b6b7-132">Yleiset järjestelmänvalvojat voivat myös palauttaa muiden järjestelmänvalvojan salasanat.</span><span class="sxs-lookup"><span data-stu-id="3b6b7-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="3b6b7-133">**En näe paikallisen integroinnin teriä salasanan nollaamisen aikana**</span><span class="sxs-lookup"><span data-stu-id="3b6b7-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="3b6b7-134">Paikallinen integrointisuljenta näkyy vain yhdistelmäympäristöissä, eli käytät salasanan palautusta paikallisen käyttäjän salasanojen käsittelemiseen.</span><span class="sxs-lookup"><span data-stu-id="3b6b7-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="3b6b7-135">Et näe tätä terää, jos:</span><span class="sxs-lookup"><span data-stu-id="3b6b7-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="3b6b7-136">Et käytä salasanan palautusta</span><span class="sxs-lookup"><span data-stu-id="3b6b7-136">You are not using password writeback</span></span>
  - <span data-ttu-id="3b6b7-137">Salasanan takaisin kirjoittamisen asennuksessa ja yhteydessä on ongelma</span><span class="sxs-lookup"><span data-stu-id="3b6b7-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="3b6b7-138">Azure AD Connectin asennuksessa ja yhteydessä on ongelma</span><span class="sxs-lookup"><span data-stu-id="3b6b7-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="3b6b7-139">Lisätietoja salasanojen palautusongelmien vianmäärityksestä on ohjeaiheessa Salasanalla [kirjoitettavan takaisin kirjoittamisen vianmääritys](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="3b6b7-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="3b6b7-140">**En tiedä, miten voin vaihtaa käyttäjän salasanan**</span><span class="sxs-lookup"><span data-stu-id="3b6b7-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="3b6b7-141">Kirjaudu Azure-portaaliin asianmukaisena järjestelmänvalvojana.</span><span class="sxs-lookup"><span data-stu-id="3b6b7-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="3b6b7-142">Siirry Käyttäjät ja **ryhmät -teriin** ja valitse **Kaikki käyttäjät.**</span><span class="sxs-lookup"><span data-stu-id="3b6b7-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="3b6b7-143">Valitse käyttäjä luettelosta.</span><span class="sxs-lookup"><span data-stu-id="3b6b7-143">Select a user from the list.</span></span>
4. <span data-ttu-id="3b6b7-144">Valitse valitulle käyttäjälle **Yleiskatsaus** ja valitse sitten komentopalkissa Palauta **salasana.**</span><span class="sxs-lookup"><span data-stu-id="3b6b7-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="3b6b7-145">Valitse Palauta **salasana -painike** ja noudata näyttöön tulevia ohjeita.</span><span class="sxs-lookup"><span data-stu-id="3b6b7-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="3b6b7-146">Vain Azure-portaalin kautta suoritetut **nollaukset tukevat** salasanan palautusta.</span><span class="sxs-lookup"><span data-stu-id="3b6b7-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="3b6b7-147">**Palautan paikallisen käyttäjän salasanan Office 365 -hallintaportaalista tai Office 365 -mobiilisovelluksesta, mutta käyttäjä ei vieläkään pysty kirjautumaan sisään**</span><span class="sxs-lookup"><span data-stu-id="3b6b7-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="3b6b7-148">Salasanasuojaa ei tueta tässä portaalissa.</span><span class="sxs-lookup"><span data-stu-id="3b6b7-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="3b6b7-149">Palauta käyttäjän salasana uudelleen Azure-portaalissa.</span><span class="sxs-lookup"><span data-stu-id="3b6b7-149">Reset the user's password again in the Azure portal.</span></span>
