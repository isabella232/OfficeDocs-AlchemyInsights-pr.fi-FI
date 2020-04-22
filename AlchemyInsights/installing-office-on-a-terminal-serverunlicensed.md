---
title: Officen asentaminen päätepalvelimeen - Käyttöoikeudeton
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 7252efdc0f55b8923e685ec89f9b3c63882aa6b0
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763214"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="c4cf8-102">Officen asentaminen päätepalvelimeen</span><span class="sxs-lookup"><span data-stu-id="c4cf8-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="c4cf8-103">Microsoft 365 Apps for enterprisen käyttöönotto Windows Serverissä etätyöpöytäpalveluiden (RDS) avulla, aiemmin päätepalvelut:</span><span class="sxs-lookup"><span data-stu-id="c4cf8-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="c4cf8-104">Sinulla on oltava Microsoft 365 -tilaus, joka sisältää Microsoft 365 Apps for Enterprise -sovelluksen, kuten Office 365 Enterprise E3 tai Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="c4cf8-105">Microsoft 365 Apps for Business- ja Microsoft 365 Apps for Business Premium -palvelupaketit eivät sisällä Microsoft 365 Apps for enterprise -palvelupaketteja.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="c4cf8-106">Sinun on otettava [käyttöön jaetun tietokoneen aktivointi](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="c4cf8-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="c4cf8-107">Jos haluat asentaa Microsoft 365 Apps for enterprisen RDS:ään Microsoft 365 -hallintakeskuksesta, ***joka käyttää asennuksen oletusasetuksia,*** toimi seuraavasti.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="c4cf8-108">Voit myös ladata ja suorittaa [Microsoftin tuki- ja palautusavustajan,](https://aka.ms/SaRA_OfficeSCA_M365Portal) jos haluat asentaa Microsoft 365 Apps for enterprisen jaetun tietokoneen aktivointitilassa.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="c4cf8-109">Tarkista, mitä Microsoft 365 -tilausta sinulla on.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="c4cf8-110">Lue lisää</span><span class="sxs-lookup"><span data-stu-id="c4cf8-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="c4cf8-111">Vaihda tarvittaessa toiseen Microsoft 365 -tilaukseen.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="c4cf8-112">Lue lisää</span><span class="sxs-lookup"><span data-stu-id="c4cf8-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="c4cf8-113">Jos Office on jo asennettu RDS-palvelimeen muiden Microsoft 365 -tilausten avulla, poista sen asennus.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="c4cf8-114">Esimerkiksi menemällä Ohjauspaneeli \> Poista ohjelma.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="c4cf8-115">Poista asennus [Microsoftin tuki- ja palautusavustajan](https://aka.ms/SARA-OfficeUninstall-Alchemy) avulla, jos kohtaat ongelmia.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="c4cf8-116">Kirjaudu RDS-palvelimessa Microsoft 365 -hallintakeskukseen järjestelmänvalvojan tilillä ja [asenna Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="c4cf8-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="c4cf8-117">Kun Office on asennettu, ***älä avaa tai kirjaudu sisään*** mihinkään Office-sovellukseen.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="c4cf8-118">Ota jaettu tietokone aktivointi käyttöön RDS-palvelimessa muokkaamalla rekisteriä seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="c4cf8-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="c4cf8-119">Napsauta näytön vasemmassa alakulmassa olevaa Windows-painiketta hiiren kakkospainikkeella ja valitse Suorita.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="c4cf8-120">Kirjoita Avaa-ruutuun **regedit**ja valitse sitten OK.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="c4cf8-121">Valitse Kyllä, kun sinua kehotetaan sallimaan Rekisterieditorin tehdä muutoksia laitteeseesi.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="c4cf8-122">Lisää rekisterieditorissa **SharedComputerLicensing-merkkijono,** jonka asetus on 1 kohdassa HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="c4cf8-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="c4cf8-123">Kirjaudu RDS-palvelimessa ***sisään loppukäyttäjänä*** ja [varmista, että jaetun tietokoneen aktivointi on otettu käyttöön Microsoft 365 Apps for enterprise -palvelussa.](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded)</span><span class="sxs-lookup"><span data-stu-id="c4cf8-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="c4cf8-124">Lisätietoja edellytyksistä, asennusohjeista ja mukautettujen asennusten ohjeista Officen käyttöönottotyökalun avulla on ohjeaiheessa [Microsoft 365 Apps for enterprise -sovelluksen käyttöönotto etätyöpöytäpalveluiden avulla](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="c4cf8-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="c4cf8-125">Lisätietoja jaetun tietokoneen aktivointiin liittyvien virheiden korjaamisesta on [ohjeaiheessa Microsoft 365 Apps for enterprise -sovelluksen jaetun tietokoneen aktivoinnin ongelmien vianmääritys](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="c4cf8-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  