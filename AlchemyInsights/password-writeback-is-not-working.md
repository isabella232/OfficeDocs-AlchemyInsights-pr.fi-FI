---
title: Salasanan takaisin kirjoittaminen ei toimi
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
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243364"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="19507-102">Salasanan takaisin kirjoittaminen ei toimi</span><span class="sxs-lookup"><span data-stu-id="19507-102">Password Writeback is not working</span></span>

<span data-ttu-id="19507-103">**Minulla on ongelmia salasanan takaisin kirjoittamisen määrittämisessä**</span><span class="sxs-lookup"><span data-stu-id="19507-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="19507-104">Salasanan takaisin kirjoittaminen on premium-ominaisuus.</span><span class="sxs-lookup"><span data-stu-id="19507-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="19507-105">Varmista, että ymmärrät käyttöoikeusvaatimukset:</span><span class="sxs-lookup"><span data-stu-id="19507-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="19507-106">Sinulla on oltava vähintään yksi käyttöoikeus määritettynä organisaatiossasi</span><span class="sxs-lookup"><span data-stu-id="19507-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="19507-107">**Vain pilvipalvelun käyttäjät** – mikä tahansa Office 365 (O365) maksettu SKU tai Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="19507-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="19507-108">**Pilvi- ja/tai** paikalliskäyttäjät – Azure AD Premium P1 tai P2, Enterprise Mobility + Security (EMS) tai Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="19507-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="19507-109">Lisätietoja käyttöoikeusvaatimuksista on kohdassa [Azure AD:n omatoimista salasanan vaihtoa koskevat käyttöoikeusvaatimukset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="19507-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="19507-110">Sinulla on vähintään yksi järjestelmänvalvojan tili ja yksi testikäyttäjätili, jolla on jokin asianmukainen käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="19507-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="19507-111">Azure AD Connect on kytkettävä ensisijaiseen toimialueen ohjauskoneemulaattoriin, jotta salasanan palautus toimii.</span><span class="sxs-lookup"><span data-stu-id="19507-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="19507-112">Voit määrittää Azure AD Connectin käyttämään ensisijaista toimialueen  ohjauskonetta napsauttamalla Active Directory -synkronointiyhdistimen ominaisuuksia hiiren kakkospainikkeella ja valitsemalla sitten **määritä hakemisto-osiot.**</span><span class="sxs-lookup"><span data-stu-id="19507-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="19507-113">Etsi sieltä toimialueen ohjauskoneen **yhteysasetukset** -osio ja valitse ruutu, jossa on vain ensisijaiset **toimialueen ohjauskoneet.**</span><span class="sxs-lookup"><span data-stu-id="19507-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="19507-114">Jos ensisijainen DC ei ole PDC-emulaattori, Azure AD Connect ottaa edelleen yhteyttä PDC:hen salasanan palautusta varten.</span><span class="sxs-lookup"><span data-stu-id="19507-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="19507-115">Salasanan vaihtaminen on määritetty ja otettu käyttöön vuokraajassa.</span><span class="sxs-lookup"><span data-stu-id="19507-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="19507-116">Lisätietoja on kohdassa Azure [AD -salasanojen palauttamisen salliminen käyttäjille.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)</span><span class="sxs-lookup"><span data-stu-id="19507-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="19507-117">Varmista, että salasanan palautus otetaan käyttöön järjestelmänvalvojan tilillä pilvipalvelun järjestelmänvalvojan tilillä (luotu Azure AD:ssä, ei paikallisessa AD:ssä)</span><span class="sxs-lookup"><span data-stu-id="19507-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="19507-118">Käytössäsi on yksittäinen tai usean puuryhmän AD-ympäristö, jossa on Windows Server 2008 R2, Windows Server 2012 tai Windows Server 2012 R2, johon on asennettu uusimmat Service Pack -paketit</span><span class="sxs-lookup"><span data-stu-id="19507-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="19507-119">Sinulla on Azure AD Connect -työkalu asennettuna ja olet valmistellut AD-ympäristön synkronointia varten pilvipalveluun.</span><span class="sxs-lookup"><span data-stu-id="19507-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="19507-120">Ennen kuin testaat salasanan takaisin kirjoittamisen, varmista, että suoritat ensin täydellisen tuonnin ja täyden synkronoinnin sekä AD:stä että Azure AD:stä Azure AD Connectissa.</span><span class="sxs-lookup"><span data-stu-id="19507-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="19507-121">Lisätietoja on ohjeaiheessa Täyden synkronoinnin ja täyden [tuonnin luominen Azure AD Connectissa](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="19507-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="19507-122">**Minulla on ongelmia salasanan takaisin kirjoittamisen yhteydessä**</span><span class="sxs-lookup"><span data-stu-id="19507-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="19507-123">[Azure AD Connectin](https://www.microsoft.com/download/details.aspx?id=47594) uusimman version lataaminen ja ottaminen käyttöön</span><span class="sxs-lookup"><span data-stu-id="19507-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="19507-124">Palomuurin määritys: Azure AD Connect -työkalulla (1.1.443 ja sitä uudempi versio) on **lähtevien HTTPS-yhteyksien** käyttö:</span><span class="sxs-lookup"><span data-stu-id="19507-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="19507-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="19507-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="19507-126">servicebus.windows.networks</span><span class="sxs-lookup"><span data-stu-id="19507-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="19507-127">Salli käyttämättömän yhteyden jatkuminen vähintään 2–3 minuutin ajan</span><span class="sxs-lookup"><span data-stu-id="19507-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="19507-128">**Minulla on edelleen ongelmia salasanan takaisin kirjoittamisen kanssa**</span><span class="sxs-lookup"><span data-stu-id="19507-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="19507-129">Jos sinulla on edelleen ongelmia, kokeile poistaa salasanan palautuspalvelu käytöstä ja ottaa se uudelleen käyttöön Azure AD Connect -työkalussa.</span><span class="sxs-lookup"><span data-stu-id="19507-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="19507-130">Lisätietoja on ohjeaiheessa Salasanan [palautusten poistaminen käytöstä ja ottaminen uudelleen käyttöön](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="19507-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
