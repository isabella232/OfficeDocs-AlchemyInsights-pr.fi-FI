---
title: Office-sovellusten automaattisten päivitysten hallinta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1743"
- "9000140"
ms.openlocfilehash: 5c56c3adcc9a06db43d4df6f367657cb8ff0c8c8
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439331"
---
# <a name="control-automatic-updates-for-office-apps"></a><span data-ttu-id="ad704-102">Office-sovellusten automaattisten päivitysten hallinta</span><span class="sxs-lookup"><span data-stu-id="ad704-102">Control automatic updates for Office Apps</span></span>

<span data-ttu-id="ad704-103">Oletusarvon mukaan Office-sovellusten päivitykset ladataan automaattisesti ja otetaan käyttöön taustalla ilman käyttäjän toimia.</span><span class="sxs-lookup"><span data-stu-id="ad704-103">By default, updates for Office Apps are downloaded automatically and applied in the background without any user intervention.</span></span> <span data-ttu-id="ad704-104">Järjestelmänvalvojat voivat kuitenkin hallita päivitysten asennusta Office Update -asetusten avulla.</span><span class="sxs-lookup"><span data-stu-id="ad704-104">However, administrators can control how updates are applied by using Office Update settings.</span></span> <span data-ttu-id="ad704-105">Päivitysasetusten avulla järjestelmänvalvojat voivat ottaa automaattiset päivitykset käyttöön tai poistaa ne käytöstä, näyttää tai piilottaa **Päivitä nyt** -painikkeen Officessa, asettaa päivityksen määräajat ja paljon muuta.</span><span class="sxs-lookup"><span data-stu-id="ad704-105">Update settings allow administrators to enable or disable automatic updates, show or hide the **Update Now** button in Office, set update deadlines, and more.</span></span> <span data-ttu-id="ad704-106">Lisätietoja on seuraavissa ohjeissa:</span><span class="sxs-lookup"><span data-stu-id="ad704-106">For detailed information, see:</span></span>

- [<span data-ttu-id="ad704-107">Officen päivitysasetusten määrittäminen</span><span class="sxs-lookup"><span data-stu-id="ad704-107">Configure update settings for Office</span></span>](https://docs.microsoft.com/deployoffice/configure-update-settings-for-office-365-proplus)  
- [<span data-ttu-id="ad704-108">Officen automaattinen päivitys ei ole käytössä</span><span class="sxs-lookup"><span data-stu-id="ad704-108">Automatic updating for Office is not enabled</span></span>](https://support.microsoft.com/help/2753538/automatic-updating-for-office-2013-and-office-2016-click-to-run-is-not)  
- [<span data-ttu-id="ad704-109">Officen päivitystavan määrittäminen asennuksen jälkeen</span><span class="sxs-lookup"><span data-stu-id="ad704-109">Define how Office is updated after it's installed</span></span>](https://docs.microsoft.com/deployoffice/configuration-options-for-the-office-2016-deployment-tool#updates-element)

<span data-ttu-id="ad704-110">Voit tarkistaa asiakastietokoneeseen käytetyt päivitysasetukset seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="ad704-110">To review the existing updates settings applied to a client machine, follow these steps:</span></span>

1. <span data-ttu-id="ad704-111">Auki Arkisto Julkaisija luona astuva jotta **Alku**  >  **Ajelu**  >  **holhoojahallitus**.</span><span class="sxs-lookup"><span data-stu-id="ad704-111">Open the Registry Editor by going to **Start** > **Run** > **regedit**.</span></span>
2. <span data-ttu-id="ad704-112">Siirry seuraavaan sijaintiin ja tarkista Office Update -asetukset:</span><span class="sxs-lookup"><span data-stu-id="ad704-112">Switch to the following location and review the Office Update settings:</span></span>  
    <span data-ttu-id="ad704-113">a.</span><span class="sxs-lookup"><span data-stu-id="ad704-113">a.</span></span> <span data-ttu-id="ad704-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\\\-kansio</span><span class="sxs-lookup"><span data-stu-id="ad704-114">HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Office\</span></span>  
    <span data-ttu-id="ad704-115">b.</span><span class="sxs-lookup"><span data-stu-id="ad704-115">b.</span></span> <span data-ttu-id="ad704-116">ClickToRun\Configuration (ValitseToRun\Configuration)</span><span class="sxs-lookup"><span data-stu-id="ad704-116">ClickToRun\Configuration</span></span>

<span data-ttu-id="ad704-117">**Huomautus**  Jos OfficeMgmtCOM-avain on määritetty, **Office**  >  **Office-tilin**  >  **Office-päivitykset**-kohdassa saattaa näkyä Päivitykset, joita järjestelmänvalvoja hallitsee.</span><span class="sxs-lookup"><span data-stu-id="ad704-117">**Note**  If the OfficeMgmtCOM key is set, you might see the "Updates are managed by your system administrator" message in **Office** > **Account** > **Office Updates**.</span></span> <span data-ttu-id="ad704-118">Lisätietoja on [ohjeaiheessa Microsoft 365 -sovellusten päivitysten hallinta Microsoft Endpoint Configuration Managerin avulla](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span><span class="sxs-lookup"><span data-stu-id="ad704-118">For more info, see [Manage updates to Microsoft 365 Apps with Microsoft Endpoint Configuration Manager](https://docs.microsoft.com/deployoffice/manage-updates-to-office-365-proplus-with-system-center-configuration-manager#method-1-use-office-deployment-tool-to-enable-office-365-clients-to-receive-updates-from-configuration-manager).</span></span>  