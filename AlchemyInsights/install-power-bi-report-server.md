---
title: Power BI Report Serverin asentaminen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1304"
- "2500001"
ms.openlocfilehash: 8479be2a538228b71033aca3907d3aba2f5e28fb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832091"
---
# <a name="install-power-bi-report-server"></a><span data-ttu-id="093be-102">Power BI Report Serverin asentaminen</span><span class="sxs-lookup"><span data-stu-id="093be-102">Install Power BI Report Server</span></span>

1. <span data-ttu-id="093be-103">Etsi sijainnit PowerBIReportServer.exe käynnistä asennusohjelma.</span><span class="sxs-lookup"><span data-stu-id="093be-103">Find the location of PowerBIReportServer.exe and launch the installer.</span></span>

2. <span data-ttu-id="093be-104">Valitse **Asenna Power BI Report Server**.</span><span class="sxs-lookup"><span data-stu-id="093be-104">Select **Install Power BI Report Server**.</span></span>

3. <span data-ttu-id="093be-105">Valitse asennettava versio ja valitse sitten **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="093be-105">Choose an edition to install and then select **Next**.</span></span>

4. <span data-ttu-id="093be-106">Voit valita avattavasta luettelosta joko Evaluation (Arviointi) tai Developer Edition (Kehitystyökalut).</span><span class="sxs-lookup"><span data-stu-id="093be-106">You can choose either Evaluation or Developer edition from the drop down.</span></span>  <span data-ttu-id="093be-107">Muussa tapauksessa voit antaa tuoteavaimen palvelimeen, jonka olet hankkinut joko Power BI -palvelusta tai volyymikäyttöoikeuskeskuksesta.</span><span class="sxs-lookup"><span data-stu-id="093be-107">Otherwise, you can enter a product key for the server that you acquired from either the Power BI service or the Volume License Service Center.</span></span> <span data-ttu-id="093be-108">Lisätietoja tuoteavaimen saamista varten on Ennen aloittamista -osassa.</span><span class="sxs-lookup"><span data-stu-id="093be-108">For more information about how to get your product key, see the Before you begin section.</span></span> <span data-ttu-id="093be-109">Lue ja hyväksy käyttöoikeussopimuksen ehdot ja valitse sitten **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="093be-109">Read and agree to the license terms and conditions, and then select **Next**.</span></span>

5. <span data-ttu-id="093be-110">Raporttipalvelimen tietokannan tallennusta varten on oltava tietokantamoduuli.</span><span class="sxs-lookup"><span data-stu-id="093be-110">You need to have a Database Engine available to store the report server database.</span></span> <span data-ttu-id="093be-111">Asenna **vain** raporttipalvelin valitsemalla Seuraava.</span><span class="sxs-lookup"><span data-stu-id="093be-111">Select **Next** to install the report server only.</span></span>

6. <span data-ttu-id="093be-112">Määritä raporttipalvelimen asennussijainti.</span><span class="sxs-lookup"><span data-stu-id="093be-112">Specify the install location for the report server.</span></span> <span data-ttu-id="093be-113">Jatka **valitsemalla** Asenna.</span><span class="sxs-lookup"><span data-stu-id="093be-113">Select **Install** to continue.</span></span>

7. <span data-ttu-id="093be-114">Kun määritys on onnistunut, käynnistä Reporting **Servicesin** määritysten hallinta valitsemalla Määritä raporttipalvelin.</span><span class="sxs-lookup"><span data-stu-id="093be-114">After a successful setup, select **Configure Report Server** to launch the Reporting Services Configuration Manager.</span></span>

<span data-ttu-id="093be-115">Et tarvitse SQL Server Database Engine -palvelinta asennuksen aikana.</span><span class="sxs-lookup"><span data-stu-id="093be-115">You don't need a SQL Server Database Engine server available at the time of install.</span></span> <span data-ttu-id="093be-116">Tarvitset sellaisen Reporting Servicesin määrittämiseen asennuksen jälkeen.</span><span class="sxs-lookup"><span data-stu-id="093be-116">You will need one to configure Reporting Services after install.</span></span>

<span data-ttu-id="093be-117">Lisätietoja: https://docs.microsoft.com/power-bi/report-server/install-report-server</span><span class="sxs-lookup"><span data-stu-id="093be-117">For more information: https://docs.microsoft.com/power-bi/report-server/install-report-server</span></span>
