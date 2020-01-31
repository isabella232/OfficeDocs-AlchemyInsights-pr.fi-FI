---
title: Kohteiden poistaminen SharePointista tai OneDrivesta ei onnistu
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571247"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="dee8b-102">Kohteiden poistaminen ei onnistu</span><span class="sxs-lookup"><span data-stu-id="dee8b-102">Unable to delete items</span></span>

<span data-ttu-id="dee8b-103">Säilytys käytännöt voivat aiheuttaa tämän, sinun on joko poistettava tai suljettava pois kyseinen ongelma, joka aiheuttaa tämän ongelman.</span><span class="sxs-lookup"><span data-stu-id="dee8b-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="dee8b-104">Kun säilytys käytäntö tai pito on poistettu, muutos tulee voimaan 24 tunnin kuluttua.</span><span class="sxs-lookup"><span data-stu-id="dee8b-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="dee8b-105">Varmista, että nimikkeellä ei ole [säilytys käytäntö](https://docs.microsoft.com/office365/securitycompliance/retention-policies) asetuksia.</span><span class="sxs-lookup"><span data-stu-id="dee8b-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="dee8b-106">Sivusto on saattanut ylittää tallennus rajoituksen, kasvattaa [sivuston kiintiötä](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ja poistaa kohteen.</span><span class="sxs-lookup"><span data-stu-id="dee8b-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="dee8b-107">Varmista, että kohde ei ole [kuitattu ulos](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) toiselle käyttäjälle.</span><span class="sxs-lookup"><span data-stu-id="dee8b-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="dee8b-108">Järjestelmänvalvojilla on myös käytössä [SharePoint-malleja ja käytäntöjä](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), jotka sisältävät PowerShell-komentoja, joiden avulla voit suorittaa monimutkaisia hallinta toimintoja, kuten pakottaa itsepäiset kohteet.</span><span class="sxs-lookup"><span data-stu-id="dee8b-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="dee8b-109">Poista PNP-tiedosto</span><span class="sxs-lookup"><span data-stu-id="dee8b-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="dee8b-110">Poista PNP-kansio</span><span class="sxs-lookup"><span data-stu-id="dee8b-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="dee8b-111">Poista PNP-luettelo kohde</span><span class="sxs-lookup"><span data-stu-id="dee8b-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="dee8b-112">Poista PNP-luettelo</span><span class="sxs-lookup"><span data-stu-id="dee8b-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="dee8b-113">Poista PNP-kenttä (sarake)</span><span class="sxs-lookup"><span data-stu-id="dee8b-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)