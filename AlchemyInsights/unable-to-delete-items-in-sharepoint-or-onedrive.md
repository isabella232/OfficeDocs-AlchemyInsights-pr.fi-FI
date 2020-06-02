---
title: Kohteita ei voi poistaa SharePointissa tai OneDrivessa
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
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511973"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="6eb94-102">Kohteita ei voi poistaa</span><span class="sxs-lookup"><span data-stu-id="6eb94-102">Unable to delete items</span></span>

<span data-ttu-id="6eb94-103">Säilytyskäytännöt voivat aiheuttaa tämän, sinun on joko poistettava käytöstä tai suljettava pois vastaava pito, joka aiheuttaa tämän ongelman.</span><span class="sxs-lookup"><span data-stu-id="6eb94-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="6eb94-104">Kun säilytyskäytäntö tai pito on poistettu, muutoksen voimaantulo voi kestää jopa 24 tuntia.</span><span class="sxs-lookup"><span data-stu-id="6eb94-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="6eb94-105">Varmista, että kohteessa ei ole [säilytyskäytäntöasetuksia.](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)</span><span class="sxs-lookup"><span data-stu-id="6eb94-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="6eb94-106">Sivusto on saattanut ylittää tallennusrajan, suurentaa [sivuston kiintiötä](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ja poistaa kohteen.</span><span class="sxs-lookup"><span data-stu-id="6eb94-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="6eb94-107">Varmista, että kohdetta ei ole [kuitattu ulos](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) toiselle käyttäjälle.</span><span class="sxs-lookup"><span data-stu-id="6eb94-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="6eb94-108">Lopuksi järjestelmänvalvojat voivat käyttää [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) -toimintoa, joka sisältää PowerShell-komentojen kirjaston, jonka avulla voit suorittaa monimutkaisia hallintatoimintoja, kuten pakottaa itsepintaisten kohteiden poistamisen.</span><span class="sxs-lookup"><span data-stu-id="6eb94-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="6eb94-109">Poista PNP-tiedosto</span><span class="sxs-lookup"><span data-stu-id="6eb94-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="6eb94-110">Poista PNP-kansio</span><span class="sxs-lookup"><span data-stu-id="6eb94-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="6eb94-111">Poista PNP-luettelokohde</span><span class="sxs-lookup"><span data-stu-id="6eb94-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="6eb94-112">Poista PNP-luettelo</span><span class="sxs-lookup"><span data-stu-id="6eb94-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="6eb94-113">PNP-kentän poistaminen (sarake)</span><span class="sxs-lookup"><span data-stu-id="6eb94-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)