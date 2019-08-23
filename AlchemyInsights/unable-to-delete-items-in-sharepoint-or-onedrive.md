---
title: Voi poistaa kohteita SharePoint-tai OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: b25e6d144dcefcfed4258e78ad5cfd4089ba7d1e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36558650"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="e6d57-102">Kohteiden poistaminen ei onnistu</span><span class="sxs-lookup"><span data-stu-id="e6d57-102">Unable to delete items</span></span>

<span data-ttu-id="e6d57-103">Poistetaan kohteita SharePoint ongelmia?</span><span class="sxs-lookup"><span data-stu-id="e6d57-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="e6d57-104">Varmista aina, että sinulla on [riittävät oikeudet](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) poistaa kohteen tai poistaa kohteen [Sivustokokoelman järjestelmänvalvoja](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) -yritys.</span><span class="sxs-lookup"><span data-stu-id="e6d57-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="e6d57-105">Varmistaa, että ei ole [säilytyskäytäntö](https://docs.microsoft.com/office365/securitycompliance/retention-policies) asetukset kohteessa.</span><span class="sxs-lookup"><span data-stu-id="e6d57-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="e6d57-106">Varmista kohde on [kuitattu ulos](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) toiselle käyttäjälle.</span><span class="sxs-lookup"><span data-stu-id="e6d57-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="e6d57-107">Lisäksi järjestelmänvalvojat voivat käyttää [SharePoint-kuviot ja käytäntöjä](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) joka sisältää kirjaston PowerShellin komennot, joiden avulla voit tehdä monimutkaisia hallinnan toimintoja kuten pakottaa stubborn poistosta.</span><span class="sxs-lookup"><span data-stu-id="e6d57-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="e6d57-108">PNP-tiedoston poistaminen</span><span class="sxs-lookup"><span data-stu-id="e6d57-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="e6d57-109">PNP-kansion poistaminen</span><span class="sxs-lookup"><span data-stu-id="e6d57-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="e6d57-110">Poista luettelokohteen PNP</span><span class="sxs-lookup"><span data-stu-id="e6d57-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="e6d57-111">Poista PNP-luettelo</span><span class="sxs-lookup"><span data-stu-id="e6d57-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="e6d57-112">Poista Plug and Play-kenttä (sarake)</span><span class="sxs-lookup"><span data-stu-id="e6d57-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)