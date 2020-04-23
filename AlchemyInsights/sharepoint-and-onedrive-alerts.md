---
title: SharePoint- ja OneDrive-ilmoitusten vastaanottamisen viivästykset
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: fb7ab6e8139c46d89b1cae1ee0ab9b9a601c8b64
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741998"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="87707-102">SharePoint- ja OneDrive-ilmoitusten vastaanottamisen viivästykset</span><span class="sxs-lookup"><span data-stu-id="87707-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="87707-103">Tarkista ensin roskapostikansio sähköpostistasi.</span><span class="sxs-lookup"><span data-stu-id="87707-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="87707-104">Jos **kaikki useiden tiedostojen tai kirjastojen ilmoitukset viivästyvät,** tarkista, onko SharePointissa tai Exchangessa mahdollisesti ilmenneitä tietoja tai tapahtumia Palvelun [kunto -koontinäytössä.](https://portal.office.com/adminportal/home?ref=/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="87707-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="87707-105">Ongelma saattaa johtua SharePoint-hälytysominaisuudesta tai viiveistä Exchangen kautta.</span><span class="sxs-lookup"><span data-stu-id="87707-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="87707-106">Huomaa myös, toimitetaanko muita sähköpostiviestejä – jos ei, ongelma liittyy todennäköisesti Exchange-viiveisiis.</span><span class="sxs-lookup"><span data-stu-id="87707-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="87707-107">Jos **tietyn tiedoston tai kirjaston yksittäistä ilmoitusta ei toimiteta,** yritä poistaa se ja luoda se uudelleen.</span><span class="sxs-lookup"><span data-stu-id="87707-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="87707-108">Lisätietoja ilmoituksen luomisesta on ohjeaiheessa [SharePoint-ilmoitusten hallinta, tarkasteleminen tai poistaminen.](https://support.microsoft.com/office/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)</span><span class="sxs-lookup"><span data-stu-id="87707-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="87707-109">Hälytyksiä ei voi lähettää jakeluryhmään.</span><span class="sxs-lookup"><span data-stu-id="87707-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="87707-110">Vain suojaus- ja O365-ryhmiä tuetaan.</span><span class="sxs-lookup"><span data-stu-id="87707-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="87707-111">Hälytyssähköpostimalleja ei voi mukauttaa.</span><span class="sxs-lookup"><span data-stu-id="87707-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="87707-112">Sinun on käytettävä Microsoft Flow'ta tai SharePoint Designer -työnkulkua.</span><span class="sxs-lookup"><span data-stu-id="87707-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
