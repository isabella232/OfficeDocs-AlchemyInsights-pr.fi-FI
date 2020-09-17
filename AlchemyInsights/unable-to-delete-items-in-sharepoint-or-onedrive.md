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
ms.openlocfilehash: fd12115214cc28b822cf7fa57fe9b86f76f7beb1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806108"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="04e67-102">Kohteiden poistaminen ei onnistu</span><span class="sxs-lookup"><span data-stu-id="04e67-102">Unable to delete items</span></span>

<span data-ttu-id="04e67-103">Säilytys käytännöt voivat aiheuttaa tämän ongelman, sinun on joko poistettava käytöstä tai jätettävä tämä ongelma huomiotta.</span><span class="sxs-lookup"><span data-stu-id="04e67-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="04e67-104">Kun säilytys käytännön tai pito on poistettu, muutoksen voimaan jääminen voi kestää jopa 24 tuntia.</span><span class="sxs-lookup"><span data-stu-id="04e67-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="04e67-105">Varmista, että kohteessa ei ole [säilytys käytännön](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) määritystä.</span><span class="sxs-lookup"><span data-stu-id="04e67-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="04e67-106">Sivuston tallennus tila on ehkä ylitetty, kasvata [sivuston kiintiötä](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) ja Poista kohde.</span><span class="sxs-lookup"><span data-stu-id="04e67-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="04e67-107">Varmista, ettei kohdetta ole [kuitattu ulos](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) toiselle käyttäjälle.</span><span class="sxs-lookup"><span data-stu-id="04e67-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="04e67-108">Lopuksi järjestelmänvalvojat voivat käyttää [SharePoint-malleja ja-käytäntöjä](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), jotka sisältävät PowerShell-komentoja, joiden avulla voit suorittaa monimutkaisia hallinta toimintoja, kuten pakottaa poistamaan itsepäisiä kohteita.</span><span class="sxs-lookup"><span data-stu-id="04e67-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="04e67-109">PNP-tiedoston poistaminen</span><span class="sxs-lookup"><span data-stu-id="04e67-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="04e67-110">PNP-kansion poistaminen</span><span class="sxs-lookup"><span data-stu-id="04e67-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="04e67-111">PNP-luettelon kohteen poistaminen</span><span class="sxs-lookup"><span data-stu-id="04e67-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="04e67-112">PNP-luettelon poistaminen</span><span class="sxs-lookup"><span data-stu-id="04e67-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="04e67-113">PNP-kentän (sarakkeen) poistaminen</span><span class="sxs-lookup"><span data-stu-id="04e67-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)