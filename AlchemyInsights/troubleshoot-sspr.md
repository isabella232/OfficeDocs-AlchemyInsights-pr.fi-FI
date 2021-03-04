---
title: SSPR:n vianmääritys
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429721"
---
# <a name="troubleshoot-sspr"></a><span data-ttu-id="72eaf-102">SSPR:n vianmääritys</span><span class="sxs-lookup"><span data-stu-id="72eaf-102">Troubleshoot SSPR</span></span>

<span data-ttu-id="72eaf-103">**Minulla on ongelmia salasanan palauttamisen määrittämisessä**</span><span class="sxs-lookup"><span data-stu-id="72eaf-103">**I'm having trouble configuring password reset**</span></span>

- <span data-ttu-id="72eaf-104">Jos olet järjestelmänvalvoja ja haluat, miten omatoiminen salasanan vaihto otetaan käyttöön, katso [ohjeet SSPR:n](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)käyttöönottamisen opetusohjelmasta organisaation salasanan palauttamisen määrittämiseen.</span><span class="sxs-lookup"><span data-stu-id="72eaf-104">If you are administrator and looking for how to enable self-service password reset, see [Tutorial enable SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), to configure password reset for your organization.</span></span> <span data-ttu-id="72eaf-105">Voit myös tarkistaa [käyttöoikeusvaatimukset.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="72eaf-105">You may also want to review the [licensing requirements](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span> <span data-ttu-id="72eaf-106">Sinulla on oltava vähintään yksi käyttöoikeus määritettynä organisaatiossasi.</span><span class="sxs-lookup"><span data-stu-id="72eaf-106">You must have at least one license assigned in your organization.</span></span>
    - <span data-ttu-id="72eaf-107">**Vain pilvipalvelun käyttäjät** – mikä tahansa Office 365 (O365) maksettu SKU tai Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="72eaf-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="72eaf-108">**Pilvi- ja/tai** paikalliskäyttäjät – Azure AD Premium P1 tai P2, Enterprise Mobility + Security (EMS) tai Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="72eaf-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
- <span data-ttu-id="72eaf-109">Lisätietoja omatoimisen salasanan palauttamisesta on usein [kysytyissä kysymyksissä.](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="72eaf-109">For additional questions about self-service password reset, review [our FAQ](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="72eaf-110">**Näyttöön tulee virhesanoma**</span><span class="sxs-lookup"><span data-stu-id="72eaf-110">**I'm getting an error message**</span></span>

<span data-ttu-id="72eaf-111">Tässä artikkelissa on yleisiä virheitä ja niiden ratkaisuja: [Omatoiminen salasanan](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support) vaihtaminen -vianmääritys</span><span class="sxs-lookup"><span data-stu-id="72eaf-111">Review this article to find common errors and their solutions: [Troubleshoot self-service password reset](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="72eaf-112">**Minulla on ongelmia salasanan palautuskäytännön kanssa**</span><span class="sxs-lookup"><span data-stu-id="72eaf-112">**I'm having a problem with my password reset policy**</span></span>

- <span data-ttu-id="72eaf-113">Jos salasanan palautuskäytäntö ei toimi odotetulla tavalla tai jos sinulla on kysyttävää salasanan palautuskäytännöistä, lue tämä artikkeli: Salasanakäytännöt ja [-rajoitukset Azure Active Directoryssa.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="72eaf-113">If your password reset policy is not behaving as expected, or if you have questions about password reset policies, review this article: [Password policies and restrictions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="72eaf-114">Salasanan palautuskäytännöt eivät koske järjestelmänvalvojille.</span><span class="sxs-lookup"><span data-stu-id="72eaf-114">Password reset policies do not apply to administrators.</span></span> <span data-ttu-id="72eaf-115">Microsoft ottaa käyttöön vahvan kaksiportaisen salasanan palautuskäytännön kaikissa Azure-järjestelmänvalvojan roolissa.</span><span class="sxs-lookup"><span data-stu-id="72eaf-115">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role.</span></span> <span data-ttu-id="72eaf-116">Varmista, että testaat käyttäjää, joka ei ole järjestelmänvalvoja.</span><span class="sxs-lookup"><span data-stu-id="72eaf-116">Make sure that you are testing with a user who is not an administrator.</span></span> <span data-ttu-id="72eaf-117">Lisätietoja järjestelmänvalvojan palautuskäytäntöön on tässä artikkelissa: Järjestelmänvalvojan [palautuskäytäntöjen erot.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)</span><span class="sxs-lookup"><span data-stu-id="72eaf-117">For more information on the administrator reset policy, see this article: [Administrator reset policy differences](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).</span></span>

<span data-ttu-id="72eaf-118">**En halua käyttäjien rekisteröitävän muita suojaustietoja salasanan palauttamista varten**</span><span class="sxs-lookup"><span data-stu-id="72eaf-118">**I don't want my users to register additional security info for password reset**</span></span>

<span data-ttu-id="72eaf-119">Voit lisätä käyttäjien tiedot (sähköposti- ja puhelinmääritteet) valmiiksi ohjelmointirajapinnan, PowerShellin tai Azure AD Connectin avulla.</span><span class="sxs-lookup"><span data-stu-id="72eaf-119">You can pre-populate data (email and phone attributes) for your users using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="72eaf-120">Lue lisätietoja seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="72eaf-120">To learn how read:</span></span>

- [<span data-ttu-id="72eaf-121">Salasanan palauttamisen käyttöönotto ilman, että käyttäjien on rekisteröidyttävä</span><span class="sxs-lookup"><span data-stu-id="72eaf-121">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [<span data-ttu-id="72eaf-122">Mitä tietoja salasanan nollaaminen käyttää</span><span class="sxs-lookup"><span data-stu-id="72eaf-122">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="72eaf-123">**Haluan, että käyttäjät rekisteröivät lisäsuojaustietonsa salasanan palauttamista varten**</span><span class="sxs-lookup"><span data-stu-id="72eaf-123">**I want my users to register their additional security info for password reset**</span></span>

1. <span data-ttu-id="72eaf-124">Anna käyttäjien rekisteröidä suojaustietonsa omatoimista salasanan vaihtoa varten ohjaamalla heidät [aka.ms/ssprsetup.](https://mysignins.microsoft.com/security-info)</span><span class="sxs-lookup"><span data-stu-id="72eaf-124">Have your users register their security info for self service password reset by directing them to [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).</span></span>
1. <span data-ttu-id="72eaf-125">Kun käyttäjä (käyttäjä tai järjestelmänvalvoja) täyttää tiedot, ohjaa käyttäjä [aka.ms/sspr](https://passwordreset.microsoftonline.com/) jotta käyttäjät voivat vaihtaa omat salasanansa.</span><span class="sxs-lookup"><span data-stu-id="72eaf-125">After data is populated for the user (by the user or by the admin), direct your user to [aka.ms/sspr](https://passwordreset.microsoftonline.com/) so your users can be empowered to reset their own passwords.</span></span>
1. <span data-ttu-id="72eaf-126">Jos käyttäjillä on edelleen ongelmia, he ovat todennäköisimmin **liitettyjä käyttäjiä** tai salasanojen **hash-salasanojen synkronoinnissa.**</span><span class="sxs-lookup"><span data-stu-id="72eaf-126">If users are still experiencing problems they are most likely **federated** or **password hash synched** users.</span></span> <span data-ttu-id="72eaf-127">Tämä tarkoittaa, että salasanan palautuspalvelussa on todennäköisesti ongelma.</span><span class="sxs-lookup"><span data-stu-id="72eaf-127">This means there is likely a problem with the Password Writeback service.</span></span>