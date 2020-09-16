---
title: SharePointin ilmoitus ilmoitukset eivät ole toimitettuina
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: f4002dc865fb7a03b07a9256709b947d6d774cb0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751240"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="7730f-102">SharePointin ilmoitus ilmoitukset eivät ole toimitettuina</span><span class="sxs-lookup"><span data-stu-id="7730f-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="7730f-103">Tarkista roska posti-kansio sähkö postista, koska joskus ilmoitukset voivat mennä sinne.</span><span class="sxs-lookup"><span data-stu-id="7730f-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="7730f-104">Tarkista, että **Kaikki ilmoitukset eivät ole toimitettuina** tai jos **yksittäistä ilmoitusta** tietystä tiedostosta tai kirjastosta ei toimiteta.</span><span class="sxs-lookup"><span data-stu-id="7730f-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="7730f-105">**Yksittäisiä hälytyksiä ei toimiteta**: Jos tietyn tiedoston tai kirjaston yksittäistä ilmoitusta ei toimiteta, voit yrittää poistaa sen ja luoda sen uudelleen.</span><span class="sxs-lookup"><span data-stu-id="7730f-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="7730f-106">Jos haluat luoda ilmoituksen uudelleen [, Katso SharePoint-ilmoitusten hallinta, tarkastelu tai poistaminen](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) .</span><span class="sxs-lookup"><span data-stu-id="7730f-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="7730f-107">**Kaikkia ilmoituksia ei toimiteta**: Jos kaikki useiden tiedostojen tai kirjastojen ilmoitukset eivät ole toimitettuina, tutustu [palvelun kunnon koonti näyttöön](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) ja tarkista kaikki SharePoint-tai Exchange-palvelussa mahdollisesti ilmenevät varoitukset ja häiriöt.</span><span class="sxs-lookup"><span data-stu-id="7730f-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="7730f-108">Ongelma voi olla SharePoint-ilmoitusten ominaisuus tai viiveet Sähkö posti viesteissä Exchangen kautta.</span><span class="sxs-lookup"><span data-stu-id="7730f-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="7730f-109">On myös tärkeää huomata, toimitetaanko muita Sähkö posti viestejä, ja jos näin ei ole, ongelma on todennäköisesti Exchange-viiveiden kanssa.</span><span class="sxs-lookup"><span data-stu-id="7730f-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="7730f-110">Usein kysyttyjä kysymyksiä ilmoituksista:</span><span class="sxs-lookup"><span data-stu-id="7730f-110">FAQ on alerts:</span></span>

- <span data-ttu-id="7730f-111">Ilmoituksia ei voi lähettää jakeluun-ryhmälle, vain suojausta ja O365 ryhmiä tuetaan.</span><span class="sxs-lookup"><span data-stu-id="7730f-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="7730f-112">Et voi mukauttaa ilmoitusten Sähkö posti malleja. sinun on käytettävä Microsoft FLOW'TA tai SharePoint Designer-työn kulkua niiden saavuttamiseksi.</span><span class="sxs-lookup"><span data-stu-id="7730f-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

## <a name="related-topics"></a><span data-ttu-id="7730f-113">Aiheeseen liittyviä ohjeita</span><span class="sxs-lookup"><span data-stu-id="7730f-113">Related Topics</span></span>

<span data-ttu-id="7730f-114">Haluatko kokeilla Microsoft Flow'ta SharePoint Onlinessa?</span><span class="sxs-lookup"><span data-stu-id="7730f-114">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="7730f-115">Työn kulun luominen</span><span class="sxs-lookup"><span data-stu-id="7730f-115">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="7730f-116">SharePoint ja Flow</span><span class="sxs-lookup"><span data-stu-id="7730f-116">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
