---
title: Officen asentaminen Terminal Serveriin-käyttö oikeus ei ole lisensoitu
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
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/25/2019
ms.locfileid: "37205406"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="a0473-102">Officen asentaminen pääte palvelimeen</span><span class="sxs-lookup"><span data-stu-id="a0473-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="a0473-103">Jos haluat ottaa Office 365 ProPlusin käyttöön Windows Serverissä käyttämällä Remote Desktop Servicesiä (RDS), aiemmin nimettyjä pääte palveluita:</span><span class="sxs-lookup"><span data-stu-id="a0473-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="a0473-104">Sinulla on oltava Office 365-suunnitelma, joka sisältää Office 365 ProPlusin, kuten Office 365 Enterprise E3 tai Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="a0473-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="a0473-105">Office 365 Business-ja Office 365 Business Premium-paketit eivät sisällä Office 365 ProPlusia.</span><span class="sxs-lookup"><span data-stu-id="a0473-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="a0473-106">Sinun on otettava käyttöön [jaetun tieto koneen Akti vointi](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="a0473-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="a0473-107">Jos haluat asentaa Office 365 ProPlus RDS Microsoft 365 hallinta keskukseen, ***joka käyttää asennuksen oletus asetukset***, toimi seuraavasti.</span><span class="sxs-lookup"><span data-stu-id="a0473-107">If you want to install Office 365 ProPlus on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="a0473-108">Voit myös ladata ja suorittaa [Microsoftin tuki-ja palautus avustajan](https://aka.ms/SaRA_OfficeSCA_M365Portal) ja asentaa Office 365 ProPlusin jaettuun tieto koneen aktivointi tilaan.</span><span class="sxs-lookup"><span data-stu-id="a0473-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Office 365 ProPlus in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="a0473-109">Tarkista, mitä Office 365-suunnitelma sinulla on.</span><span class="sxs-lookup"><span data-stu-id="a0473-109">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="a0473-110">Lue, miten</span><span class="sxs-lookup"><span data-stu-id="a0473-110">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="a0473-111">Vaihda tarvittaessa toiseen Office 365-suunnitelmaan.</span><span class="sxs-lookup"><span data-stu-id="a0473-111">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="a0473-112">Lue, miten</span><span class="sxs-lookup"><span data-stu-id="a0473-112">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="a0473-113">Jos Office on jo asennettu RDS-palvelimeen muiden Office 365-palvelu pakettien avulla, poista se.</span><span class="sxs-lookup"><span data-stu-id="a0473-113">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="a0473-114">Esimerkiksi siirtymällä ohjaus paneeliin \> Poista ohjelma.</span><span class="sxs-lookup"><span data-stu-id="a0473-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="a0473-115">Poista asennus [Microsoft Support-ja Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) -ohjelman avulla, jos ongelmia ei ole.</span><span class="sxs-lookup"><span data-stu-id="a0473-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="a0473-116">Kirjaudu RDS-palvelimella Microsoft 365-hallinta keskukseen järjestelmänvalvojan tilillä ja [Asenna Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span><span class="sxs-lookup"><span data-stu-id="a0473-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="a0473-117">Kun Office on asennettu, ***Älä avaa tai Kirjaudu*** mihinkään Office-sovelluksiin.</span><span class="sxs-lookup"><span data-stu-id="a0473-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="a0473-118">Ota käyttöön jaetun tieto koneen Akti vointi RDS-palvelimessa muokkaamalla rekisteriä tekemällä seuraavat toimet:</span><span class="sxs-lookup"><span data-stu-id="a0473-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="a0473-119">Napsauta hiiren kakkos painikkeella näytön vasemmassa alakulmassa olevaa Windows-painiketta ja valitse Suorita.</span><span class="sxs-lookup"><span data-stu-id="a0473-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="a0473-120">Kirjoita Avaa-ruutuun **regedit**ja valitse sitten OK.</span><span class="sxs-lookup"><span data-stu-id="a0473-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="a0473-121">Valitse Kyllä, kun sinua pyydetään sallimaan rekisteri editorin tehdä muutoksia laitteeseesi.</span><span class="sxs-lookup"><span data-stu-id="a0473-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="a0473-122">Lisää rekisteri editorissa **Sharedcomputerlicensing** -merkki jono arvo, jonka asetus on 1 kohdassa HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="a0473-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="a0473-123">Kirjaudu sisään RDS-palvelimessa ***loppu käyttäjänä*** ja [Varmista, että Office 365 ProPlusin jaetun tieto koneen Akti vointi on käytössä](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="a0473-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="a0473-124">Lisä tietoja edellytyksistä, asennus ohjeista ja ohjeista mukautetuista asennuksista Officen käyttöönotto työkalun avulla on artikkelissa [office 365 ProPlusin käyttöönotto Etätyöpöytäpalvelujen avulla](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="a0473-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="a0473-125">Voit korjata jaettuun tieto koneen Akti vointiin liittyviä virheitä kohdasta [Office 365 ProPlusin jaetun tieto koneen Akti voinnin ongelmien vian määritys](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="a0473-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  