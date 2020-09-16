---
title: Viiveet SharePoint-ja OneDrive-ilmoitusten vastaanottamisessa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727240"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="61db8-102">Viiveet SharePoint-ja OneDrive-ilmoitusten vastaanottamisessa</span><span class="sxs-lookup"><span data-stu-id="61db8-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="61db8-103">Tarkista ensin roska posti-tai roska posti-kansio sähkö postista.</span><span class="sxs-lookup"><span data-stu-id="61db8-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="61db8-104">Jos **Kaikki useiden tiedostojen tai kirjastojen ilmoitukset viivästyvät**, tarkista [palvelun kunnon koonti näytöstä](https://portal.office.com/adminportal/home?ref=/servicehealth) , että SharePoint-tai Exchange-palvelussa mahdollisesti esiintyvät varoitukset ja häiriöt ovat mahdollisia.</span><span class="sxs-lookup"><span data-stu-id="61db8-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="61db8-105">Ongelma voi olla SharePoint-ilmoitusten ominaisuus tai viiveet Sähkö posti viesteissä Exchangen kautta.</span><span class="sxs-lookup"><span data-stu-id="61db8-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="61db8-106">Huomaa myös, onko muita Sähkö posti viestejä toimitettu – jos näin ei ole, ongelma aiheutuu todennäköisesti Exchange-viiveistä.</span><span class="sxs-lookup"><span data-stu-id="61db8-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="61db8-107">Jos **tietyn tiedoston tai kirjaston yksittäistä ilmoitusta ei toimiteta**, yritä poistaa se ja luoda se uudelleen.</span><span class="sxs-lookup"><span data-stu-id="61db8-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="61db8-108">Jos haluat luoda ilmoituksen uudelleen [, Katso SharePoint-ilmoitusten hallinta, tarkastelu tai poistaminen](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) .</span><span class="sxs-lookup"><span data-stu-id="61db8-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="61db8-109">Hälytyksiä ei voi lähettää jakelun ryhmälle.</span><span class="sxs-lookup"><span data-stu-id="61db8-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="61db8-110">Vain suojausta ja O365 ryhmiä tuetaan.</span><span class="sxs-lookup"><span data-stu-id="61db8-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="61db8-111">Et voi mukauttaa ilmoitusten Sähkö posti malleja.</span><span class="sxs-lookup"><span data-stu-id="61db8-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="61db8-112">Sinun on käytettävä Microsoft Flow'ta tai SharePoint Designer-työn kulkua niiden saavuttamiseksi.</span><span class="sxs-lookup"><span data-stu-id="61db8-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
