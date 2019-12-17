---
title: Poistetun tiedoston tai kansion palauttaminen
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: 2702837bff2c0a465dde2c090a44e02747cc85ec
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051062"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="4f28f-102">Poistetun tiedoston tai kansion palauttaminen</span><span class="sxs-lookup"><span data-stu-id="4f28f-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="4f28f-103">SharePoint Online säilyttää kaiken sisällön varmuus kopiot 14 lisä päivän ajan varsi naisen poiston jälkeen.</span><span class="sxs-lookup"><span data-stu-id="4f28f-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="4f28f-104">Jos sisältöä ei voi palauttaa roska korin tai tiedostojen palauttamisen avulla, järjestelmänvalvoja voi ottaa yhteyttä Microsoftin tukeen ja pyytää palautusta milloin tahansa 14 päivän ikkunan sisällä.</span><span class="sxs-lookup"><span data-stu-id="4f28f-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="4f28f-105">Varmuus kopioiden palautukset voidaan suorittaa vain sivustokokoelmille tai alisivustoille, ei tietyille tiedostoille, luetteloille tai kirjastoille.</span><span class="sxs-lookup"><span data-stu-id="4f28f-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="4f28f-106">Kun poistat kohteen tai sivuston SharePointista, sitä ei poisteta heti.</span><span class="sxs-lookup"><span data-stu-id="4f28f-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="4f28f-107">Poistetut kohteet menevät roska koriin tietyn ajan.</span><span class="sxs-lookup"><span data-stu-id="4f28f-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="4f28f-108">Tänä aikana voit palauttaa poistetut kohteet alkuperäiseen sijaintiinsa.</span><span class="sxs-lookup"><span data-stu-id="4f28f-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="4f28f-109">Lisä tietoja on alla olevissa linkeissä.</span><span class="sxs-lookup"><span data-stu-id="4f28f-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="4f28f-110">[Palauta SharePoint-sivuston roska korin kohteet](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span><span class="sxs-lookup"><span data-stu-id="4f28f-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span></span>

[<span data-ttu-id="4f28f-111">Palauta poistetut tiedostot tai kansiot OneDrivessa</span><span class="sxs-lookup"><span data-stu-id="4f28f-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="4f28f-112">Poistettujen sivustokokoelmaan (mukaan lukien ryhmä, viestintä ja muut sivustot) palauttaminen</span><span class="sxs-lookup"><span data-stu-id="4f28f-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="4f28f-113">Poistetun OneDrive-sivuston palauttaminen</span><span class="sxs-lookup"><span data-stu-id="4f28f-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="4f28f-114">Jos kyseessä on joukko roska kori, järjestelmänvalvojat voivat harkita [SharePoint Online PnP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)-toimintojen käyttämistä.</span><span class="sxs-lookup"><span data-stu-id="4f28f-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="4f28f-115">**Tiedostojen palauttaminen-ominaisuus**</span><span class="sxs-lookup"><span data-stu-id="4f28f-115">**Files Restore feature**</span></span>

<span data-ttu-id="4f28f-116">Jos paljon OneDrivea tai SharePoint-tiedostoja poistetaan, korvataan, vioittuu tai haitta ohjelmilta tartuttaa, voit palauttaa koko OneDriven tai SharePoint-kirjastosi aiempaan aikaan käyttämällä tiedostojen palauttaminen-toimintoa.</span><span class="sxs-lookup"><span data-stu-id="4f28f-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="4f28f-117">OneDrive-kirjaston palauttaminen</span><span class="sxs-lookup"><span data-stu-id="4f28f-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="4f28f-118">Asiakirja kirjaston palauttaminen</span><span class="sxs-lookup"><span data-stu-id="4f28f-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

