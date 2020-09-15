---
title: Officen asentaminen Terminal Serveriin-käyttöoikeudeton
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663114"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="7202e-102">Officen asentaminen pääte palvelimeen</span><span class="sxs-lookup"><span data-stu-id="7202e-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="7202e-103">Jos haluat ottaa käyttöön Microsoft 365-sovelluksia yritys käyttöön Windows-palvelimessa käyttämällä Etätyöpöytäpalveluja (RDS), aiemmin nimettyjä pääte palveluja:</span><span class="sxs-lookup"><span data-stu-id="7202e-103">For deploying Microsoft 365 Apps for enterprise on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="7202e-104">Sinulla on oltava Microsoft 365-tilaus, joka sisältää Microsoft 365-sovellukset yritykselle, kuten Office 365 Enterprise E3 tai Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="7202e-104">You must have a Microsoft 365 subscription that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="7202e-105">Yritys käyttöön tarkoitettuja Microsoft 365-sovelluksia ja Microsoft 365-sovellukset eivät sisällä Microsoft 365-sovelluksia yritys käyttöön.</span><span class="sxs-lookup"><span data-stu-id="7202e-105">The Microsoft 365 Apps for business and Microsoft 365 Apps for business Premium plans do not include Microsoft 365 Apps for enterprise.</span></span>

- <span data-ttu-id="7202e-106">Sinun on otettava käyttöön [jaettujen tieto koneiden Akti vointi](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="7202e-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

<span data-ttu-id="7202e-107">Jos haluat asentaa Microsoft 365-sovelluksia Enterprise on RDS-sovellukseen Microsoft 365-hallinta keskuksesta, ***jossa käytetään oletusarvoisia asennus asetuksia***, noudata seuraavia ohjeita.</span><span class="sxs-lookup"><span data-stu-id="7202e-107">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps.</span></span>

> [!TIP]
> <span data-ttu-id="7202e-108">Voit myös ladata ja suorittaa [Microsoftin tuki-ja palautus avustajan](https://aka.ms/SaRA_OfficeSCA_M365Portal) ja asentaa Microsoft 365-sovelluksia yritys käyttöön jaetussa tieto koneen aktivointi tilassa.</span><span class="sxs-lookup"><span data-stu-id="7202e-108">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>
  
1. <span data-ttu-id="7202e-109">Tarkista, mikä Microsoft 365-tilaus sinulla on.</span><span class="sxs-lookup"><span data-stu-id="7202e-109">Check what Microsoft 365 subscription you have.</span></span> [<span data-ttu-id="7202e-110">Lisä tietoja</span><span class="sxs-lookup"><span data-stu-id="7202e-110">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="7202e-111">Vaihda tarvittaessa toiseen Microsoft 365-tila ukseen.</span><span class="sxs-lookup"><span data-stu-id="7202e-111">If necessary, switch to a different Microsoft 365 subscription.</span></span> [<span data-ttu-id="7202e-112">Lisä tietoja</span><span class="sxs-lookup"><span data-stu-id="7202e-112">Learn how</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. <span data-ttu-id="7202e-113">Jos Office on jo asennettu RDS-palvelimeen käyttämällä muita Microsoft 365-paketteja, poista sen asennus.</span><span class="sxs-lookup"><span data-stu-id="7202e-113">If Office is already installed on the RDS server using any other Microsoft 365 subscriptions, uninstall it.</span></span> <span data-ttu-id="7202e-114">Esimerkiksi siirtymällä ohjaus paneeliin voit \> poistaa ohjelman asennuksen.</span><span class="sxs-lookup"><span data-stu-id="7202e-114">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="7202e-115">Poista asennus [Microsoftin tuki-ja palautus avustajan avulla,](https://aka.ms/SARA-OfficeUninstall-Alchemy) jos käytät ongelmia.</span><span class="sxs-lookup"><span data-stu-id="7202e-115">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="7202e-116">Kirjaudu RDS-palvelimessa Microsoft 365-hallinta keskukseen järjestelmänvalvojan tilillä ja [Asenna microsoft 365-sovellukset](https://portal.office.com/OLS/MySoftware.aspx)yrityksille.</span><span class="sxs-lookup"><span data-stu-id="7202e-116">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="7202e-117">Kun Office on asennettu, ***Älä avaa tai Kirjaudu sisään*** mihinkään Office-sovelluksiin.</span><span class="sxs-lookup"><span data-stu-id="7202e-117">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="7202e-118">Ota RDS-palvelimessa käyttöön tieto koneen yhteinen Akti vointi muokkaamalla rekisteriä noudattamalla seuraavia ohjeita:</span><span class="sxs-lookup"><span data-stu-id="7202e-118">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="7202e-119">Napsauta näytön vasemmassa alakulmassa olevaa Windows-painiketta hiiren kakkos painikkeella ja valitse Suorita.</span><span class="sxs-lookup"><span data-stu-id="7202e-119">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="7202e-120">Kirjoita Avaa-ruutuun **regedit**ja valitse sitten OK.</span><span class="sxs-lookup"><span data-stu-id="7202e-120">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="7202e-121">Valitse Kyllä, kun ohjelma kysyy, sallitaanko rekisteri editorin tehdä muutoksia laitteeseesi.</span><span class="sxs-lookup"><span data-stu-id="7202e-121">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="7202e-122">Lisää rekisteri editorissa **Sharedcomputerlicensing** -arvo, jonka asetus on 1, HKEY_LOCAL_MACHINE \Microsoft\microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="7202e-122">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="7202e-123">Kirjaudu sisään RDS-palvelimessa ***loppu käyttäjänä*** ja [Varmista, että Microsoft 365-sovellukset on otettu käyttöön jaetussa tieto koneessa](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span><span class="sxs-lookup"><span data-stu-id="7202e-123">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>

<span data-ttu-id="7202e-124">Lisä tietoja Office-käyttöönotto työkalun käyttö edellytyksistä, määritys ohjeista ja mukautetuista asennuksista on artikkelissa [Microsoft 365-sovellusten käyttöönotto yritys käyttöön tarkoitettuja Etätyöpöytäpalveluja](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)käyttämällä.</span><span class="sxs-lookup"><span data-stu-id="7202e-124">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>
  
<span data-ttu-id="7202e-125">Jos haluat korjata jaettuihin tieto koneen Akti vointiin liittyviä ongelmia, Katso lisä tietoja artikkelista ongelmien [vian määritys jaetussa tieto koneessa Microsoft 365-sovellusten Akti vointi yrityksessä](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span><span class="sxs-lookup"><span data-stu-id="7202e-125">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
  