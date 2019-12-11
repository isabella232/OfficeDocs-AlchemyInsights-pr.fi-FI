---
title: Office 365 ProPlusin käyttöönotto jaettuun käyttöön RDS-, Terminal Server-tai VDI-palvelimessa
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959457"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="45494-102">Office 365 ProPlusin käyttöönotto jaettuun käyttöön RDS-, Terminal Server-tai VDI-palvelimessa</span><span class="sxs-lookup"><span data-stu-id="45494-102">Deploying Office 365 ProPlus for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="45494-103">Voit ottaa Office 365 ProPlusin käyttöön käyttämällä Remote Desktop Servicesia (RDS), jonka nimi oli aiemmin Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="45494-103">To deploy Office 365 ProPlus using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
- <span data-ttu-id="45494-104">Sinulla on oltava Microsoft 365 for Business-suunnitelma tai Office 365-suunnitelma, joka sisältää Office 365 ProPlusin, kuten Office 365 Enterprise E3 tai Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="45494-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE] 
   > <span data-ttu-id="45494-105">Office 365 Business-ja Office 365 Business Premium-paketit eivät sisällä Office 365 ProPlusia.</span><span class="sxs-lookup"><span data-stu-id="45494-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>
- <span data-ttu-id="45494-106">Sinun on otettava käyttöön [jaetun tieto koneen Akti vointi](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="45494-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

> [!NOTE]
> <span data-ttu-id="45494-107">Voit myös ladata ja suorittaa [Microsoftin tuki-ja palautus avustajan](https://aka.ms/SaRA_OfficeSCA_M365Portal) ja asentaa Office 365 ProPlusin jaettuun tieto koneen aktivointi tilaan.</span><span class="sxs-lookup"><span data-stu-id="45494-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>

<span data-ttu-id="45494-108">Lisä tietoja edellytyksistä, asennus ohjeista ja mukautettujen asennusten ohjeista Officen käyttöönotto työkalun avulla on artikkelissa [office 365 ProPlusin käyttöönotto Etätyöpöytäpalvelujen avulla](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="45494-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>

<span data-ttu-id="45494-109">Jaettuun tieto koneen Akti vointiin liittyvien virheiden korjaaminen:</span><span class="sxs-lookup"><span data-stu-id="45494-109">To fix errors related to shared computer activation:</span></span>
- <span data-ttu-id="45494-110">Katso [Office 365 ProPlusin jaetun tieto koneen Akti voinnin ongelmien vian määritys](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="45494-110">See [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
- <span data-ttu-id="45494-111">Katso [Office 365 ProPlus-aktivointi tilan palauttaminen](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="45494-111">See [Reset Office 365 ProPlus activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="45494-112">Jos haluat asentaa Office 365 ProPlus RDS Microsoft 365 hallinta keskukseen, ***joka käyttää asennuksen oletus asetukset***, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="45494-112">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1.  <span data-ttu-id="45494-113">Tarkista, mitä Office 365-suunnitelma sinulla on.</span><span class="sxs-lookup"><span data-stu-id="45494-113">Check what Office 365 plan you have.</span></span> <span data-ttu-id="45494-114">[Ohjeet](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="45494-114">[Learn how](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2.  <span data-ttu-id="45494-115">Vaihda tarvittaessa toiseen Office 365-suunnitelmaan.</span><span class="sxs-lookup"><span data-stu-id="45494-115">If necessary, switch to a different Office 365 plan.</span></span> <span data-ttu-id="45494-116">[Ohjeet](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="45494-116">[Learn how](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).</span></span>
3.  <span data-ttu-id="45494-117">Jos Office on jo asennettu RDS-palvelimeen muiden Office 365-palvelu pakettien avulla, poista se.</span><span class="sxs-lookup"><span data-stu-id="45494-117">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="45494-118">Esimerkiksi siirtymällä **ohjaus paneeliin** > **Poista ohjelma**.</span><span class="sxs-lookup"><span data-stu-id="45494-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="45494-119">Poista asennus [Microsoft Support-ja Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) -ohjelman avulla, jos ongelmia ei ole.</span><span class="sxs-lookup"><span data-stu-id="45494-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4.  <span data-ttu-id="45494-120">Kirjaudu RDS-palvelimella Microsoft 365-hallinta keskukseen järjestelmänvalvojan tilillä ja [Asenna Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="45494-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5.  <span data-ttu-id="45494-121">Kun Office on asennettu, ***Älä avaa tai Kirjaudu*** mihinkään Office-sovelluksiin.</span><span class="sxs-lookup"><span data-stu-id="45494-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6.  <span data-ttu-id="45494-122">Ota käyttöön jaetun tieto koneen Akti vointi RDS-palvelimessa muokkaamalla rekisteriä tekemällä seuraavat toimet:</span><span class="sxs-lookup"><span data-stu-id="45494-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="45494-123">Napsauta hiiren kakkos painikkeella näytön vasemmassa alakulmassa olevaa Windows-painiketta ja valitse **Suorita**.</span><span class="sxs-lookup"><span data-stu-id="45494-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="45494-124">Kirjoita Avaa-ruutuun **regedit**ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="45494-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="45494-125">Valitse **Kyllä** , kun sinua pyydetään sallimaan rekisteri editorin tehdä muutoksia laitteeseesi.</span><span class="sxs-lookup"><span data-stu-id="45494-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="45494-126">Lisää rekisteri editorissa **Sharedcomputerlicensing** -merkki jono arvo, jonka asetus on 1 kohdassa HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="45494-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="45494-127">Kirjaudu sisään RDS-palvelimessa ***loppu käyttäjänä*** ja [Varmista, että Office 365 ProPlusin jaetun tieto koneen Akti vointi on käytössä](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="45494-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

