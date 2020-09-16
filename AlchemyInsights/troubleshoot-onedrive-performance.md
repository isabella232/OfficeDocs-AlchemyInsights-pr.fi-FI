---
title: OneDrive-suoritus kyvyn vian määritys
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 4699f6113acd70b4778f9feeaeec012ff8fdd63f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757882"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="e3485-102">OneDrive-suoritus kyvyn vian määritys</span><span class="sxs-lookup"><span data-stu-id="e3485-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="e3485-103">Jos käytössäsi on odotettua hitaampi synkronointi tai samankaltaisia ongelmia OneDriven kanssa:</span><span class="sxs-lookup"><span data-stu-id="e3485-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="e3485-104">Varmista, että [palvelun kunnon koonti näytössä](https://portal.office.com/adminportal/home?ref=/servicehealth)ei ole tunnettuja ongelmia.</span><span class="sxs-lookup"><span data-stu-id="e3485-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="e3485-105">[Ota tiedostot käyttöön pyydettäessä](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) , jotta voit käyttää kaikkia tiedostojasi OneDrivessa tarvitsematta ladata niitä kaikkia ja käyttää laitteessa tallennus tilaa.</span><span class="sxs-lookup"><span data-stu-id="e3485-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="e3485-106">Tarkista verkon suunnittelun ja suoritus kyvyn [parhaat käytännöt](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) .</span><span class="sxs-lookup"><span data-stu-id="e3485-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="e3485-107">[Suurenna latauksen ja latauksen nopeutta](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), etenkin jos synkronoit laitetta ensimmäisen kerran.</span><span class="sxs-lookup"><span data-stu-id="e3485-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="e3485-108">Jos synkronoit kirjastoa, jossa on yli 100 000 kohdetta, OneDrive-synkronointi saattaa tuntua pitkään jumittuneen tai tila näyttää, että se käsittelee 0KB/xMB. "</span><span class="sxs-lookup"><span data-stu-id="e3485-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="e3485-109">[Lue lisä tietoja yli 100 000-tiedostojen synkronoinnista](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) sekä [onedriven tuetuista 300 000-tiedostojen rajasta](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="e3485-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="e3485-110">Kun käyttäjä on ylittänyt käyttö rajoitukset, SharePoint Online-tili ei enää enää pyydä kyseistä käyttäjä tiliä lyhyeksi ajaksi.</span><span class="sxs-lookup"><span data-stu-id="e3485-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="e3485-111">Kaikki käyttäjän toiminnot ovat kuristettu, kun kaasu vipu on voimassa.</span><span class="sxs-lookup"><span data-stu-id="e3485-111">All user actions are throttled while the throttle is in effect.</span></span>
