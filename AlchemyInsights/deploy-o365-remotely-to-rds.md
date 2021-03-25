---
title: Microsoft 365 Apps for Enterprisen käyttöönotto jaettua käyttöä varten RDS:ssä, päätepalvelimessa tai VDI:ssä
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200670"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a><span data-ttu-id="3afd1-102">Microsoft 365 Apps for Enterprisen käyttöönotto jaettua käyttöä varten RDS:ssä, päätepalvelimessa tai VDI:ssä</span><span class="sxs-lookup"><span data-stu-id="3afd1-102">Deploying Microsoft 365 Apps for enterprise for shared use on RDS, Terminal Server, or VDI</span></span>

<span data-ttu-id="3afd1-103">Microsoft 365 Apps for Enterprisen käyttöönotto etätyöpöytäpalveluja (RDS) käyttäen, aiemmin päätepalvelut:</span><span class="sxs-lookup"><span data-stu-id="3afd1-103">To deploy Microsoft 365 Apps for enterprise using Remote Desktop Services (RDS), formerly named Terminal Services:</span></span>

- <span data-ttu-id="3afd1-104">Sinulla on oltava Microsoft 365 For Business -palvelupaketti tai Office 365 -palvelupaketti, joka sisältää Microsoft 365 -sovellukset yrityksille, kuten Office 365 Enterprise E3 tai Enterprise E5.</span><span class="sxs-lookup"><span data-stu-id="3afd1-104">You must have a Microsoft 365 For Business plan or an Office 365 plan that includes Microsoft 365 Apps for enterprise, such as Office 365 Enterprise E3 or Enterprise E5.</span></span>
   > [!NOTE]
   > <span data-ttu-id="3afd1-105">Microsoft 365 Apps for Business- ja Microsoft 365 Business Standard -palvelupaketit eivät sisällä Microsoft 365 Apps for Enterprise -sovelluksia.</span><span class="sxs-lookup"><span data-stu-id="3afd1-105">The Microsoft 365 Apps for business and Microsoft 365 Business Standard plans do not include Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="3afd1-106">Sinun on otettava käyttöön [jaetun tietokoneen aktivointi.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="3afd1-106">You must enable [shared computer activation](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).</span></span>

> [!NOTE]
> <span data-ttu-id="3afd1-107">Voit myös ladata ja suorittaa [Microsoftin tuki-](https://aka.ms/SaRA_OfficeSCA_M365Portal) ja palautusavustajan, jotta voit asentaa Microsoft 365 Apps for Enterprisen jaetussa tietokoneen aktivointitilassa.</span><span class="sxs-lookup"><span data-stu-id="3afd1-107">You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.</span></span>

<span data-ttu-id="3afd1-108">Lisätietoja edellytyksistä, asennusohjeista ja mukautetuista asennuksista Officen käyttöönottotyökalun avulla on kohdassa [Microsoft 365 -sovellusten](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)käyttöönotto etätyöpöytäpalveluja käyttämällä.</span><span class="sxs-lookup"><span data-stu-id="3afd1-108">For more information on prerequisites, setup instructions, and guidance on customized installations by using the Office Deployment Tool, see [Deploy Microsoft 365 Apps for enterprise by using Remote Desktop Services](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).</span></span>

<span data-ttu-id="3afd1-109">Jaetun tietokoneen aktivointiin liittyvien virheiden korjaaminen:</span><span class="sxs-lookup"><span data-stu-id="3afd1-109">To fix errors related to shared computer activation:</span></span>

- <span data-ttu-id="3afd1-110">Katso [Microsoft 365 Apps for Enterprisen](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)jaetun tietokoneen aktivoinnin ongelmien vianmääritys.</span><span class="sxs-lookup"><span data-stu-id="3afd1-110">See [Troubleshoot issues with shared computer activation for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).</span></span>
- <span data-ttu-id="3afd1-111">Katso [Palauta aktivointitila Microsoft 365 -yrityssovelluksille](https://go.microsoft.com/fwlink/?linkid=2109218).</span><span class="sxs-lookup"><span data-stu-id="3afd1-111">See [Reset Microsoft 365 Apps for enterprise activation state](https://go.microsoft.com/fwlink/?linkid=2109218).</span></span>

<span data-ttu-id="3afd1-112">Jos haluat asentaa Microsoft 365 Apps for Enterprisen RDS:lle Microsoft 365 -hallintakeskuksesta, joka käyttää oletusasennusasetuksia, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="3afd1-112">If you want to install Microsoft 365 Apps for enterprise on RDS from the Microsoft 365 admin center, ***which uses default installation settings***, use the following steps:</span></span>

1. <span data-ttu-id="3afd1-113">Tarkista, mikä tilaus sinulla on.</span><span class="sxs-lookup"><span data-stu-id="3afd1-113">Check what subscription you have.</span></span> <span data-ttu-id="3afd1-114">[Ohjeet](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span><span class="sxs-lookup"><span data-stu-id="3afd1-114">[Learn how](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).</span></span>
2. <span data-ttu-id="3afd1-115">Vaihda tarvittaessa toiseen tilaukseen.</span><span class="sxs-lookup"><span data-stu-id="3afd1-115">If necessary, switch to a different subscription.</span></span> <span data-ttu-id="3afd1-116">[Ohjeet](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span><span class="sxs-lookup"><span data-stu-id="3afd1-116">[Learn how](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).</span></span>
3. <span data-ttu-id="3afd1-117">Jos Office on jo asennettu RDS-palvelimeen muiden Microsoft-tilausten avulla, poista sen asennus.</span><span class="sxs-lookup"><span data-stu-id="3afd1-117">If Office is already installed on the RDS server using any other Microsoft subscriptions, uninstall it.</span></span> <span data-ttu-id="3afd1-118">Voit esimerkiksi valita **Ohjauspaneelin Poista**  >  **ohjelman asennus**.</span><span class="sxs-lookup"><span data-stu-id="3afd1-118">For example, by going to **Control Panel** > **Uninstall a program**.</span></span> <span data-ttu-id="3afd1-119">Poista asennus [Microsoftin tuki-](https://aka.ms/SARA-OfficeUninstall-Alchemy) ja palautusavustajan avulla, jos sinulla on ongelmia.</span><span class="sxs-lookup"><span data-stu-id="3afd1-119">Uninstall using [Microsoft Support and Recovery Assistant](https://aka.ms/SARA-OfficeUninstall-Alchemy) if you're running into issues.</span></span>
4. <span data-ttu-id="3afd1-120">Kirjaudu RDS-palvelimessa Microsoft 365 -hallintakeskukseen järjestelmänvalvojan tililläsi ja asenna [Microsoft 365 Apps for Enterprise.](https://portal.office.com/OLS/MySoftware.aspx)</span><span class="sxs-lookup"><span data-stu-id="3afd1-120">On the RDS server, sign in to the Microsoft 365 admin center with your administrator account and [install Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).</span></span>
5. <span data-ttu-id="3afd1-121">Kun Office on asennettu, ***älä avaa tai kirjaudu*** sisään mihinkään Office-sovellukseen.</span><span class="sxs-lookup"><span data-stu-id="3afd1-121">After Office is installed, ***don't open or sign in*** to any Office applications.</span></span>
6. <span data-ttu-id="3afd1-122">Ota RDS-palvelimessa käyttöön jaettu tietokoneaktivointi muokkaamalla rekisteriä seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="3afd1-122">On the RDS server, enable shared computer activation by editing the registry by following these steps:</span></span>
   1. <span data-ttu-id="3afd1-123">Napsauta näytön vasemmassa alakulmassa olevaa Windows-painiketta hiiren kakkospainikkeella ja valitse **Suorita.**</span><span class="sxs-lookup"><span data-stu-id="3afd1-123">Right-click the Windows button in the lower left-corner of your screen and select **Run**.</span></span> <span data-ttu-id="3afd1-124">Kirjoita Avaa-ruutuun **regedit** ja napsauta sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="3afd1-124">In the Open box, type **regedit**, and then select **OK**.</span></span>
   2. <span data-ttu-id="3afd1-125">Valitse **Kyllä,** kun ohjelma pyytää sallimaan Rekisterieditorin tehdä muutoksia laitteeseesi.</span><span class="sxs-lookup"><span data-stu-id="3afd1-125">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
   3. <span data-ttu-id="3afd1-126">Lisää Rekisterieditorissa **SharedComputerLicensing-merkkijonoarvo,** jonka asetuksena on 1 kohdassa HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span><span class="sxs-lookup"><span data-stu-id="3afd1-126">In the Registry Editor, add a string value of **SharedComputerLicensing** with a setting of 1 under HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.</span></span>
   4. <span data-ttu-id="3afd1-127">Kirjaudu RDS-palvelimessa käyttäjänä ja varmista, että Microsoft 365 Apps for Enterprise -sovellukset ovat käytössä  [jaetun tietokoneen aktivoinnissa.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)</span><span class="sxs-lookup"><span data-stu-id="3afd1-127">On the RDS server, ***sign in as an end user*** and [verify that shared computer activation is enabled for Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).</span></span>
