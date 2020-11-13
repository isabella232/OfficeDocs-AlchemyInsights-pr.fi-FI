---
title: Kohteita ei voi poistaa SharePointissa tai OneDrivessa
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019580"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="de637-102">Kohteiden poistaminen ei onnistu</span><span class="sxs-lookup"><span data-stu-id="de637-102">Unable to delete items</span></span>

- <span data-ttu-id="de637-103">Säilytys käytännöt voivat aiheuttaa tämän ongelman, sinun on joko poistettava käytöstä tai jätettävä tämä ongelma huomiotta.</span><span class="sxs-lookup"><span data-stu-id="de637-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="de637-104">Kun säilytys käytännön tai pito on poistettu, muutoksen voimaan jääminen voi kestää jopa 24 tuntia.</span><span class="sxs-lookup"><span data-stu-id="de637-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="de637-105">Varmista, että kohteessa ei ole [säilytys käytännön](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) määritystä.</span><span class="sxs-lookup"><span data-stu-id="de637-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="de637-106">Sivuston tallennus tila on ehkä ylitetty, kasvata [sivuston kiintiötä](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ja Poista kohde.</span><span class="sxs-lookup"><span data-stu-id="de637-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

- <span data-ttu-id="de637-107">Varmista, ettei kohdetta ole [kuitattu ulos](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) toiselle käyttäjälle.</span><span class="sxs-lookup"><span data-stu-id="de637-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="de637-108">Lopuksi järjestelmänvalvojat voivat käyttää [SharePoint-malleja ja-käytäntöjä](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), jotka sisältävät PowerShell-komentoja, joiden avulla voit suorittaa monimutkaisia hallinta toimintoja, kuten pakottaa poistamaan itsepäisiä kohteita.</span><span class="sxs-lookup"><span data-stu-id="de637-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="de637-109">PNP-tiedoston poistaminen</span><span class="sxs-lookup"><span data-stu-id="de637-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="de637-110">PNP-kansion poistaminen</span><span class="sxs-lookup"><span data-stu-id="de637-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="de637-111">PNP-luettelon kohteen poistaminen</span><span class="sxs-lookup"><span data-stu-id="de637-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="de637-112">PNP-luettelon poistaminen</span><span class="sxs-lookup"><span data-stu-id="de637-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="de637-113">PNP-kentän (sarakkeen) poistaminen</span><span class="sxs-lookup"><span data-stu-id="de637-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)