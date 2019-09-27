---
title: SharePoint-ja OneDrive-hälytyksiä ei saada
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/25/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 80423791ad558fc414d50608c73f823036432e14
ms.sourcegitcommit: 5e6a805fb0b41d714ca1cf90e23b8e2daa90f90e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/26/2019
ms.locfileid: "37205519"
---
# <a name="not-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="d58d5-102">SharePoint-ja OneDrive-hälytyksiä ei saada</span><span class="sxs-lookup"><span data-stu-id="d58d5-102">Not receiving SharePoint and OneDrive alerts</span></span>

<span data-ttu-id="d58d5-103">Tarkista ensin sähkö postisi roska posti-tai roska posti kansio.</span><span class="sxs-lookup"><span data-stu-id="d58d5-103">First check the Junk or Spam folder in your email.</span></span>

<span data-ttu-id="d58d5-104">Selvitä sitten, onko **kaikkia hälytyksiä toimitettu** vai ei, jos tietystä tiedostosta tai kirjastosta ei toimiteta **yksittäistä ilmoitusta** .</span><span class="sxs-lookup"><span data-stu-id="d58d5-104">Then determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="d58d5-105">Jos **kaikkia ilmoituksia useista tiedostoista tai kirjastoista ei toimiteta**, käy [palvelun kunnon koonti näytössä](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fadmin.microsoft.com%2FAdminPortal%2FHome%23%2Fservicehealth&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) ja tarkista, onko SharePoint-tai Exchange-palvelussa mahdollisesti ilmenneitä neuvoja tai tapahtumia.</span><span class="sxs-lookup"><span data-stu-id="d58d5-105">If **all alerts from multiple files or libraries are not delivered**, visit the [Service Health dashboard](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fadmin.microsoft.com%2FAdminPortal%2FHome%23%2Fservicehealth&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="d58d5-106">Ongelma saattaa olla SharePoint-hälytys toiminto tai sähkö postien viivästyminen Exchangen kautta.</span><span class="sxs-lookup"><span data-stu-id="d58d5-106">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="d58d5-107">Huomaa myös, onko muita Sähkö posti viestin toimitetaan – jos ei, ongelma on todennäköisesti viivästyksiä.</span><span class="sxs-lookup"><span data-stu-id="d58d5-107">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="d58d5-108">Jos **tietyn tiedoston tai kirjaston yksittäistä ilmoitusta ei toimiteta**, yritä poistaa se ja luoda se uudelleen.</span><span class="sxs-lookup"><span data-stu-id="d58d5-108">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="d58d5-109">Katso [SharePoint-ilmoitusten hallinta, tarkasteleminen tai poistaminen](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2Fmanage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2%3Fui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax%2Fepn3E%3D&reserved=0) , jos haluat luoda hälytyksen uudelleen.</span><span class="sxs-lookup"><span data-stu-id="d58d5-109">See [Manage, view, or delete SharePoint alerts](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2Fmanage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2%3Fui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax%2Fepn3E%3D&reserved=0) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="d58d5-110">Ilmoituksia ei voi lähettää jakelu ryhmään.</span><span class="sxs-lookup"><span data-stu-id="d58d5-110">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="d58d5-111">Vain suojaus-ja O365-ryhmiä tuetaan.</span><span class="sxs-lookup"><span data-stu-id="d58d5-111">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="d58d5-112">Et voi mukauttaa hälytys Sähkö posti malleja.</span><span class="sxs-lookup"><span data-stu-id="d58d5-112">You cannot customize alert email templates.</span></span> <span data-ttu-id="d58d5-113">Sinun on käytettävä Microsoft Flow-tai SharePoint Designer-työn kulkua näiden tavoitteiden saavuttamiseksi.</span><span class="sxs-lookup"><span data-stu-id="d58d5-113">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
