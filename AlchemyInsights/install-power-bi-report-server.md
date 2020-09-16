---
title: Power BI-raportti palvelimen asentaminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1304"
- "2500001"
ms.openlocfilehash: 3ea596547093773ab872ca34e8dd3a4e49e59fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755092"
---
# <a name="install-power-bi-report-server"></a><span data-ttu-id="059e1-102">Power BI-raportti palvelimen asentaminen</span><span class="sxs-lookup"><span data-stu-id="059e1-102">Install Power BI Report Server</span></span>

1. <span data-ttu-id="059e1-103">Etsi PowerBIReportServer.exe sijainti ja käynnistä asennus ohjelma.</span><span class="sxs-lookup"><span data-stu-id="059e1-103">Find the location of PowerBIReportServer.exe and launch the installer.</span></span>

2. <span data-ttu-id="059e1-104">Valitse **Asenna Power BI-raportti palvelin**.</span><span class="sxs-lookup"><span data-stu-id="059e1-104">Select **Install Power BI Report Server**.</span></span>

3. <span data-ttu-id="059e1-105">Valitse asennettava versio ja valitse sitten **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="059e1-105">Choose an edition to install and then select **Next**.</span></span>

4. <span data-ttu-id="059e1-106">Voit valita joko arviointi-tai kehitys versio-kohdan avattavasta luettelosta.</span><span class="sxs-lookup"><span data-stu-id="059e1-106">You can choose either Evaluation or Developer edition from the drop down.</span></span>  <span data-ttu-id="059e1-107">Muussa tapa uksessa voit antaa joko Power BI-palvelusta tai volyymi käyttö oikeus keskuksesta hankitun palvelimen tuote avaimen.</span><span class="sxs-lookup"><span data-stu-id="059e1-107">Otherwise, you can enter a product key for the server that you acquired from either the Power BI service or the Volume License Service Center.</span></span> <span data-ttu-id="059e1-108">Lisä tietoja tuote avaimen hankkimisesta on ennen aloittamista-osiossa.</span><span class="sxs-lookup"><span data-stu-id="059e1-108">For more information about how to get your product key, see the Before you begin section.</span></span> <span data-ttu-id="059e1-109">Lue ja hyväksy käyttö oikeus sopimuksen ehdot ja valitse sitten **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="059e1-109">Read and agree to the license terms and conditions, and then select **Next**.</span></span>

5. <span data-ttu-id="059e1-110">Sinulla on oltava tieto kanta moduuli, joka on käytettävissä raportti palvelin tieto kannan tallentamiseen.</span><span class="sxs-lookup"><span data-stu-id="059e1-110">You need to have a Database Engine available to store the report server database.</span></span> <span data-ttu-id="059e1-111">Asenna vain raportti palvelin valitsemalla **Seuraava** .</span><span class="sxs-lookup"><span data-stu-id="059e1-111">Select **Next** to install the report server only.</span></span>

6. <span data-ttu-id="059e1-112">Määritä raportti palvelimen asennus sijainti.</span><span class="sxs-lookup"><span data-stu-id="059e1-112">Specify the install location for the report server.</span></span> <span data-ttu-id="059e1-113">Jatka valitsemalla **Asenna** .</span><span class="sxs-lookup"><span data-stu-id="059e1-113">Select **Install** to continue.</span></span>

7. <span data-ttu-id="059e1-114">Kun asennus on onnistunut, valitse **Määritä raportti palvelin** , jotta Reporting Servicesin määritysten vastuu henkilö käynnistetään.</span><span class="sxs-lookup"><span data-stu-id="059e1-114">After a successful setup, select **Configure Report Server** to launch the Reporting Services Configuration Manager.</span></span>

<span data-ttu-id="059e1-115">Et tarvitse asennus hetkellä käytettävissä olevaa SQL Server-tieto kanta moduulin palvelinta.</span><span class="sxs-lookup"><span data-stu-id="059e1-115">You don't need a SQL Server Database Engine server available at the time of install.</span></span> <span data-ttu-id="059e1-116">Tarvitset yhden, jos haluat määrittää Reporting Servicesin asennuksen jälkeen.</span><span class="sxs-lookup"><span data-stu-id="059e1-116">You will need one to configure Reporting Services after install.</span></span>

<span data-ttu-id="059e1-117">Lisä tietoja: https://docs.microsoft.com/power-bi/report-server/install-report-server</span><span class="sxs-lookup"><span data-stu-id="059e1-117">For more information: https://docs.microsoft.com/power-bi/report-server/install-report-server</span></span>
