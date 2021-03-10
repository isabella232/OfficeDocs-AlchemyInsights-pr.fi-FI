---
title: Ongelma salasanan vaihtamisessa
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694374"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="ff016-102">Ongelmia salasanan vaihtamisessa</span><span class="sxs-lookup"><span data-stu-id="ff016-102">Problems resetting password</span></span>

<span data-ttu-id="ff016-103">Seuraavassa on joitakin ongelmia, joita saatat kohdata salasanan vaihtamisen ja mahdollisia ratkaisuja käytettäessä:</span><span class="sxs-lookup"><span data-stu-id="ff016-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="ff016-104">**Minulla on ongelmia salasanan palauttamisessa, jota ei ole käsitelty muissa luokissa**</span><span class="sxs-lookup"><span data-stu-id="ff016-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="ff016-105">Varmista, että sinulla on oikeus vaihtaa salasanoja.</span><span class="sxs-lookup"><span data-stu-id="ff016-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="ff016-106">Vain yleiset järjestelmänvalvojat, salasanat ja käyttäjien järjestelmänvalvojat voivat vaihtaa käyttäjien salasanat.</span><span class="sxs-lookup"><span data-stu-id="ff016-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="ff016-107">Yleiset järjestelmänvalvojat voivat myös palauttaa muiden järjestelmänvalvojan salasanat.</span><span class="sxs-lookup"><span data-stu-id="ff016-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="ff016-108">Varmista, että ymmärrät käyttöoikeusvaatimukset:</span><span class="sxs-lookup"><span data-stu-id="ff016-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="ff016-109">Sinulla on oltava vähintään yksi käyttöoikeus määritettynä organisaatiossasi</span><span class="sxs-lookup"><span data-stu-id="ff016-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="ff016-110">Vain pilvipalvelun käyttäjät – mikä tahansa Office 365 (O365) maksettu SKU tai Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="ff016-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="ff016-111">Pilvi- ja/tai paikalliskäyttäjät – Azure AD Premium P1 tai P2, Enterprise Mobility + Security (EMS) tai Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="ff016-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="ff016-112">Lisätietoja käyttöoikeusvaatimuksista on artikkelissa Azure AD:n omatoimista salasanan vaihtoa [koskevat käyttöoikeusvaatimukset.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="ff016-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="ff016-113">**I'm having problems testing the password reset policy I set**</span><span class="sxs-lookup"><span data-stu-id="ff016-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="ff016-114">Viimeksi käytetyt käytännöt voivat replikoida kaikissa tietokeskuksissa ja päätepisteissä useita minuutteja.</span><span class="sxs-lookup"><span data-stu-id="ff016-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="ff016-115">Fyysinen etäisyys tietokeskuksesta vaikuttaa myös siihen, miten nopeasti muutoksia otetaan käyttöön.</span><span class="sxs-lookup"><span data-stu-id="ff016-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="ff016-116">Testaa loppukäyttäjän, ei järjestelmänvalvojan, kanssa ja pilotaa pienen käyttäjäjoukon kanssa.</span><span class="sxs-lookup"><span data-stu-id="ff016-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="ff016-117">Azure-portaalissa määritetyt käytännöt koskevat vain loppukäyttäjiä, eivät järjestelmänvalvojille.</span><span class="sxs-lookup"><span data-stu-id="ff016-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="ff016-118">Microsoft käyttää vahvaa kahden portin oletussalasanan palautuskäytäntöä kaikissa Azure-järjestelmänvalvojan roolissa (esimerkki: yleinen järjestelmänvalvoja, tukipalvelun järjestelmänvalvoja, salasanan järjestelmänvalvoja jne.)</span><span class="sxs-lookup"><span data-stu-id="ff016-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="ff016-119">Lisätietoja [järjestelmänvalvojien käytännöistä.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)</span><span class="sxs-lookup"><span data-stu-id="ff016-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="ff016-120">**Haluan ottaa salasanan palauttamisen käyttöön, mutta en halua, että käyttäjät rekisteröivät muita suojaustietoja**</span><span class="sxs-lookup"><span data-stu-id="ff016-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="ff016-121">Lisää käyttäjien tiedot valmiiksi, jotta heidän ei tarvitse!</span><span class="sxs-lookup"><span data-stu-id="ff016-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="ff016-122">- Järjestelmänvalvojana voit määrittää käyttäjien puhelin- ja sähköpostiominaisuudet ennen salasanan palauttamisen käyttöönottamista organisaatiossasi.</span><span class="sxs-lookup"><span data-stu-id="ff016-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="ff016-123">Voit tehdä tämän ohjelmointirajapinnan, PowerShellin tai Azure AD Connectin avulla.</span><span class="sxs-lookup"><span data-stu-id="ff016-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="ff016-124">Lisätietoja on seuraavassa:</span><span class="sxs-lookup"><span data-stu-id="ff016-124">More information here:</span></span>
- [<span data-ttu-id="ff016-125">Salasanan palauttamisen käyttöönotto ilman, että käyttäjien on rekisteröidyttävä</span><span class="sxs-lookup"><span data-stu-id="ff016-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="ff016-126">Mitä tietoja salasanan nollaaminen käyttää</span><span class="sxs-lookup"><span data-stu-id="ff016-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="ff016-127">**Salasanan vaihtopainike näkyy harmaana**</span><span class="sxs-lookup"><span data-stu-id="ff016-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="ff016-128">Sinulla ei ole oikeutta palauttaa tämän käyttäjän salasanoja.</span><span class="sxs-lookup"><span data-stu-id="ff016-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="ff016-129">Vain yleiset järjestelmänvalvojat, salasanat ja käyttäjien järjestelmänvalvojat voivat vaihtaa käyttäjien salasanat.</span><span class="sxs-lookup"><span data-stu-id="ff016-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="ff016-130">Yleiset järjestelmänvalvojat voivat myös palauttaa muiden järjestelmänvalvojan salasanat.</span><span class="sxs-lookup"><span data-stu-id="ff016-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="ff016-131">**I don't see the password reset blade**</span><span class="sxs-lookup"><span data-stu-id="ff016-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="ff016-132">Sinulla ei ole oikeutta vaihtaa salasanoja.</span><span class="sxs-lookup"><span data-stu-id="ff016-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="ff016-133">Vain yleiset järjestelmänvalvojat, salasanat ja käyttäjien järjestelmänvalvojat voivat vaihtaa käyttäjien salasanat.</span><span class="sxs-lookup"><span data-stu-id="ff016-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="ff016-134">Yleiset järjestelmänvalvojat voivat myös palauttaa muiden järjestelmänvalvojan salasanat.</span><span class="sxs-lookup"><span data-stu-id="ff016-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="ff016-135">**I don't see the on-premises integration blade in password reset**</span><span class="sxs-lookup"><span data-stu-id="ff016-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="ff016-136">Paikallinen integrointisuljenta näkyy vain yhdistelmäympäristöissä, eli käytät salasanan palautusta paikallisen käyttäjän salasanojen käsittelemiseen.</span><span class="sxs-lookup"><span data-stu-id="ff016-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="ff016-137">Et näe tätä terää, jos:</span><span class="sxs-lookup"><span data-stu-id="ff016-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="ff016-138">Et käytä salasanan palautusta</span><span class="sxs-lookup"><span data-stu-id="ff016-138">You are not using password writeback</span></span>
    - <span data-ttu-id="ff016-139">Salasanan takaisin kirjoittamisen asennuksessa ja yhteydessä on ongelma</span><span class="sxs-lookup"><span data-stu-id="ff016-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="ff016-140">Azure AD Connectin asennuksessa ja yhteydessä on ongelma</span><span class="sxs-lookup"><span data-stu-id="ff016-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="ff016-141">Lisätietoja salasanan palautusongelmien vianmäärityksestä on kohdassa Salasanan takaisin [kirjoittamisen vianmääritys](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="ff016-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="ff016-142">**En tiedä, miten voin vaihtaa käyttäjän salasanan**</span><span class="sxs-lookup"><span data-stu-id="ff016-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="ff016-143">Kirjaudu Azure-portaaliin asianmukaisena järjestelmänvalvojana.</span><span class="sxs-lookup"><span data-stu-id="ff016-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="ff016-144">Siirry Käyttäjät ja ryhmät -teriin ja valitse **Kaikki käyttäjät.**</span><span class="sxs-lookup"><span data-stu-id="ff016-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="ff016-145">Valitse käyttäjä luettelosta.</span><span class="sxs-lookup"><span data-stu-id="ff016-145">Select a user from the list.</span></span>
1. <span data-ttu-id="ff016-146">Valitse valitulle käyttäjälle **Yleiskatsaus** ja valitse sitten komentopalkissa Palauta **salasana.**</span><span class="sxs-lookup"><span data-stu-id="ff016-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="ff016-147">Noudata näyttöön tulevia ohjeita.</span><span class="sxs-lookup"><span data-stu-id="ff016-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="ff016-148">Vain Azure-portaalin kautta suoritetut nollaukset tukevat salasanan palautusta.</span><span class="sxs-lookup"><span data-stu-id="ff016-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="ff016-149">**Palautan paikallisen käyttäjän salasanan Office 365 -hallintaportaalista tai Office 365 -mobiilisovelluksesta, mutta käyttäjä ei vieläkään pysty kirjautumaan sisään**</span><span class="sxs-lookup"><span data-stu-id="ff016-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="ff016-150">Salasanasuojaa ei tueta tässä portaalissa.</span><span class="sxs-lookup"><span data-stu-id="ff016-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="ff016-151">Käyttäjän salasanan palauttaminen uudelleen Azure-portaalissa – portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="ff016-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

