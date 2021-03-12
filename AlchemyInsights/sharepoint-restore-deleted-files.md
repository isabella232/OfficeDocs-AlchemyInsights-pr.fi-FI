---
title: Poistetun tiedoston tai kansion palauttaminen
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: 8c7ce48f50b5c933ea15c23a486b99ad7a7f4d79
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707519"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="0b05b-102">Poistetun tiedoston tai kansion palauttaminen</span><span class="sxs-lookup"><span data-stu-id="0b05b-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="0b05b-103">SharePoint Online säilyttää kaiken sisällön varmuuskopiot vielä 14 päivän ajan todellisen poiston jälkeen.</span><span class="sxs-lookup"><span data-stu-id="0b05b-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="0b05b-104">Jos sisältöä ei voi palauttaa roskakorin tai tiedostojen palauttamisen kautta, järjestelmänvalvoja voi ottaa yhteyttä Microsoft-tukeen ja pyytää palautusta milloin tahansa 14 päivän ikkunassa.</span><span class="sxs-lookup"><span data-stu-id="0b05b-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="0b05b-105">Palautuksia voi suorittaa vain sivustokokoelmille tai alisivustoille, ei tietyille tiedostoille, luetteloille tai kirjastoille.</span><span class="sxs-lookup"><span data-stu-id="0b05b-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="0b05b-106">Kun poistat kohteen tai sivuston SharePointista, sitä ei poisteta heti.</span><span class="sxs-lookup"><span data-stu-id="0b05b-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="0b05b-107">Poistetut kohteet siirtyvät roskakoriin tietyksi ajaksi.</span><span class="sxs-lookup"><span data-stu-id="0b05b-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="0b05b-108">Tänä aikana voit palauttaa poistetut kohteet alkuperäiseen sijaintiinsa.</span><span class="sxs-lookup"><span data-stu-id="0b05b-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="0b05b-109">Lisätietoja saat alla olevista linkeistä.</span><span class="sxs-lookup"><span data-stu-id="0b05b-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="0b05b-110">[SharePoint-sivuston roskakorin kohteiden palauttaminen.](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be)</span><span class="sxs-lookup"><span data-stu-id="0b05b-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.microsoft.com/office/restore-items-in-the-recycle-bin-that-were-deleted-from-sharepoint-or-teams-6df466b6-55f2-4898-8d6e-c0dff851a0be).</span></span>

[<span data-ttu-id="0b05b-111">Poistettujen tiedostojen tai kansioiden palauttaminen OneDrivessa</span><span class="sxs-lookup"><span data-stu-id="0b05b-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="0b05b-112">Poistetun sivustokokoelman palauttaminen (mukaan lukien ryhmä-, viestintä- ja muut sivustot)</span><span class="sxs-lookup"><span data-stu-id="0b05b-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="0b05b-113">Poistetun OneDrive-sivuston palauttaminen</span><span class="sxs-lookup"><span data-stu-id="0b05b-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="0b05b-114">Järjestelmänvalvojat voivat käyttää joukko roskakoritoimintoja [SharePoint Onlinen PNP:n avulla.](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="0b05b-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="0b05b-115">**Tiedostojen palauttamisominaisuus**</span><span class="sxs-lookup"><span data-stu-id="0b05b-115">**Files Restore feature**</span></span>

<span data-ttu-id="0b05b-116">Jos poistat tai korvaat useita OneDrive- tai SharePoint-tiedostoja, tiedostot vioittuvat tai niissä on haittaohjelmia, voit palauttaa koko OneDrive- tai SharePoint-kirjaston aiempaan versioon tiedostojen palautustoiminnon avulla.</span><span class="sxs-lookup"><span data-stu-id="0b05b-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="0b05b-117">OneDrive-kirjaston palauttaminen</span><span class="sxs-lookup"><span data-stu-id="0b05b-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="0b05b-118">Tiedostokirjaston palauttaminen</span><span class="sxs-lookup"><span data-stu-id="0b05b-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

