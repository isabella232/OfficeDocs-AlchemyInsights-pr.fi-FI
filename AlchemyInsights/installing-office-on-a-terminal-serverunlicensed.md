---
title: Office asennetaan päätepalvelin - varastettu
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: edac051840594f13b22ccd83f5cd6e3da5f84cbc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36498412"
---
# <a name="installing-office-on-a-terminal-server"></a><span data-ttu-id="918e7-102">Päätepalvelimen asennuksen</span><span class="sxs-lookup"><span data-stu-id="918e7-102">Installing Office on a Terminal Server</span></span>

<span data-ttu-id="918e7-103">Voidaan ottaa käyttöön Office 365 ProPlus Windows-palvelimen käyttämällä Remote Desktop Services (RDS), nimeltään Terminal Services:</span><span class="sxs-lookup"><span data-stu-id="918e7-103">For deploying Office 365 ProPlus on a Windows Server using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>
  
- <span data-ttu-id="918e7-104">Jos sinulla on Office 365-suunnitelma, joka sisältää Office 365 ProPlus, kuten Office 365 Enterprise-E3 tai yrityksen E5.</span><span class="sxs-lookup"><span data-stu-id="918e7-104">You must have an Office 365 plan that includes Office 365 ProPlus, such as Office 365 Enterprise E3 or Enterprise E5.</span></span> <span data-ttu-id="918e7-105">Business Office 365: n ja Office 365: n Business Premium suunnitelmat eivät sisällä Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="918e7-105">The Office 365 Business and Office 365 Business Premium plans do not include Office 365 ProPlus.</span></span>

- <span data-ttu-id="918e7-106">On otettava käyttöön [jaettu tietokone aktivoiminen](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="918e7-106">You need to enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).</span></span>

<span data-ttu-id="918e7-107">Jos haluat asentaa Office 365 ProPlus RDS-Office 365-portaalin, ***joka käyttää oletusarvoisesti asennuksen asetuksia***, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="918e7-107">If you want to install Office 365 ProPlus on RDS from the Office 365 portal, ***which uses default installation settings***, follow these steps:</span></span>
  
1. <span data-ttu-id="918e7-108">Tarkista, mitä sinulla on Office 365-suunnitelma.</span><span class="sxs-lookup"><span data-stu-id="918e7-108">Check what Office 365 plan you have.</span></span> [<span data-ttu-id="918e7-109">Lue lisätietoja siitä, miten</span><span class="sxs-lookup"><span data-stu-id="918e7-109">Learn how</span></span>](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. <span data-ttu-id="918e7-110">Jos tarpeen, siirry eri Office 365: ssä.</span><span class="sxs-lookup"><span data-stu-id="918e7-110">If necessary, switch to a different Office 365 plan.</span></span> [<span data-ttu-id="918e7-111">Lue lisätietoja siitä, miten</span><span class="sxs-lookup"><span data-stu-id="918e7-111">Learn how</span></span>](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. <span data-ttu-id="918e7-112">Jos RDS-palvelimeen, joka käyttää Office 365-suunnitelmat on jo asennettu Office, poista sen asennus.</span><span class="sxs-lookup"><span data-stu-id="918e7-112">If Office is already installed on the RDS server using any other Office 365 plans, uninstall it.</span></span> <span data-ttu-id="918e7-113">Esimerkiksi siirtymällä Ohjauspaneelin \> Poista ohjelman asennus.</span><span class="sxs-lookup"><span data-stu-id="918e7-113">For example, by going to Control Panel \> Uninstall a program.</span></span> <span data-ttu-id="918e7-114">Asennuksen poisto käyttämällä [Microsoftin tuotetukeen ja palautus avustaja](https://aka.ms/SARA-OfficeUninstall-Alchemy) , jos ongelmia käytössä.</span><span class="sxs-lookup"><span data-stu-id="918e7-114">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>

4. <span data-ttu-id="918e7-115">RDS-palvelimen kirjautuminen järjestelmänvalvojana ja [Asenna Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx)Office 365-portaaliin.</span><span class="sxs-lookup"><span data-stu-id="918e7-115">On the RDS server, sign in to the Office 365 portal with your administrator account and [install Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).</span></span>

5. <span data-ttu-id="918e7-116">Kun Office on asennettu, ***Älä avaa tai kirjautua sisään*** Office-sovelluksia.</span><span class="sxs-lookup"><span data-stu-id="918e7-116">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>

6. <span data-ttu-id="918e7-117">RDS-palvelimen käyttöön jaetun tietokoneen aktivointi muokkaamalla rekisteriä seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="918e7-117">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>

1. <span data-ttu-id="918e7-118">Napsauta näytön vasemmassa alakulmassa olevaa Windows-painiketta ja valitse Suorita.</span><span class="sxs-lookup"><span data-stu-id="918e7-118">Right-click the Windows button in the lower left-hand corner of your screen and select Run.</span></span> <span data-ttu-id="918e7-119">Kirjoita Avaa-ruutuun **regedit**ja valitse OK.</span><span class="sxs-lookup"><span data-stu-id="918e7-119">In the Open box, type **regedit**, and then select OK.</span></span>

2. <span data-ttu-id="918e7-120">Valitse Kyllä, kun kehotetaan sallimaan Registry Editor tehdä muutoksia laitteen.</span><span class="sxs-lookup"><span data-stu-id="918e7-120">Select Yes when prompted to allow Registry Editor to make changes to your device.</span></span>

3. <span data-ttu-id="918e7-121">Registry Editor Lisää merkkijonoarvo on **SharedComputerLicensing** , joka on asetettu 1 kohdassa HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="918e7-121">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>

7. <span data-ttu-id="918e7-122">RDS-palvelin, ***Kirjaudu loppukäyttäjälle*** ja [että jaetun tietokoneen aktivointi on otettu käyttöön Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span><span class="sxs-lookup"><span data-stu-id="918e7-122">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).</span></span>

<span data-ttu-id="918e7-123">Lisätietoja edellytykset, asennusohjeita ja ohjeita mukautettujen asennusten avulla Office Deployment Tool-työkalua on [Ottaa käyttöön Office 365 ProPlus Etätyöpöytäpalveluiden avulla](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span><span class="sxs-lookup"><span data-stu-id="918e7-123">For more details on prerequisites, setup instructions and guidance on customized installations by using the Office Deployment Tool, please see [Deploy Office 365 ProPlus by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).</span></span>
  
<span data-ttu-id="918e7-124">Jaetun tietokoneen aktivointi liittyvien virheiden korjaamiseen on [jaetun tietokoneen aktivointi Office 365 ProPlus ongelmien vianmääritys](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span><span class="sxs-lookup"><span data-stu-id="918e7-124">To fix errors related to shared computer activation, please see [Troubleshoot issues with shared computer activation for Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).</span></span>
  