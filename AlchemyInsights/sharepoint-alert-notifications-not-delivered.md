---
title: SharePoint-ilmoitusilmoituksia ei toimitettu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: 363f3c79a3b62f3017e6c873f1be3dd195cab883
ms.sourcegitcommit: 5296874062b16f945d9a7a7a9ab29ec53686310b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/21/2020
ms.locfileid: "44343074"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="6a17b-102">SharePoint-ilmoitusilmoituksia ei toimitettu</span><span class="sxs-lookup"><span data-stu-id="6a17b-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="6a17b-103">Tarkista roskapostin ROSKAPOSTI-kansio, sillä joskus hälytykset saattavat mennä sinne.</span><span class="sxs-lookup"><span data-stu-id="6a17b-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="6a17b-104">Määritä, **että kaikkia hälytyksiä ei toimiteta** tai jos tietyn tiedoston tai kirjaston **yksittäistä ilmoitusta** ei toimiteta.</span><span class="sxs-lookup"><span data-stu-id="6a17b-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="6a17b-105">**Yksittäisiä hälytyksiä ei toimiteta:** Jos tietyn tiedoston tai kirjaston yksittäistä ilmoitusta ei toimiteta, voit yrittää poistaa sen ja luoda sen uudelleen.</span><span class="sxs-lookup"><span data-stu-id="6a17b-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="6a17b-106">Lisätietoja ilmoituksen luomisesta on ohjeaiheessa [SharePoint-ilmoitusten hallinta, tarkasteleminen tai poistaminen.](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)</span><span class="sxs-lookup"><span data-stu-id="6a17b-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="6a17b-107">**Kaikkia hälytyksiä ei toimiteta:** Jos kaikkia useiden tiedostojen tai kirjastojen ilmoituksia ei toimiteta, tarkista SharePointin tai Exchangen yhteydessä mahdollisesti ilmenevistä tiedotteista/tapahtumista [palvelun kunnon hallintapaneelista.](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="6a17b-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="6a17b-108">Ongelma voi johtua SharePoint-hälytysominaisuudesta tai viiveistä Exchangen kautta.</span><span class="sxs-lookup"><span data-stu-id="6a17b-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="6a17b-109">On myös tärkeää huomata, toimitetaanko muuta sähköpostia, ja jos ei, ongelma liittyy todennäköisesti Exchangen viivästyksiin.</span><span class="sxs-lookup"><span data-stu-id="6a17b-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="6a17b-110">Usein kysyttyjä kysymyksiä hälytyksistä:</span><span class="sxs-lookup"><span data-stu-id="6a17b-110">FAQ on alerts:</span></span>

- <span data-ttu-id="6a17b-111">Hälytyksiä ei voi lähettää jakeluryhmälle, vain suojaus- ja O365-ryhmiä tuetaan.</span><span class="sxs-lookup"><span data-stu-id="6a17b-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="6a17b-112">Hälytyssähköpostimalleja ei voi mukauttaa. sinun on käytettävä Microsoft FLOW- tai SharePoint Designer -työnkulkua niiden saavuttamiseksi.</span><span class="sxs-lookup"><span data-stu-id="6a17b-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

## <a name="related-topics"></a><span data-ttu-id="6a17b-113">Aiheeseen liittyviä aiheita</span><span class="sxs-lookup"><span data-stu-id="6a17b-113">Related Topics</span></span>

<span data-ttu-id="6a17b-114">Haluatko kokeilla Microsoft Flow'ta SharePoint Onlinessa?</span><span class="sxs-lookup"><span data-stu-id="6a17b-114">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="6a17b-115">Luo työnkulku</span><span class="sxs-lookup"><span data-stu-id="6a17b-115">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="6a17b-116">SharePoint ja Flow</span><span class="sxs-lookup"><span data-stu-id="6a17b-116">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
