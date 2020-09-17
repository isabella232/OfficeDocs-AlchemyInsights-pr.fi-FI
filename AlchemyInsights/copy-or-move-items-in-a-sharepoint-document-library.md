---
title: Kohteiden kopioiminen tai siirtäminen SharePoint-tiedosto kirjastossa
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "454"
- "5300013"
ms.assetid: 592f502a-493f-4bf4-adc3-5bc8aea87bb5
ms.openlocfilehash: d7aa865a6b3db0871a57313dd7d6f5b0213ca0e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47807116"
---
# <a name="copy-or-move-items-in-a-sharepoint-document-library"></a><span data-ttu-id="c9691-102">Kohteiden kopioiminen tai siirtäminen SharePoint-tiedosto kirjastossa</span><span class="sxs-lookup"><span data-stu-id="c9691-102">Copy or move items in a SharePoint document library</span></span>

<span data-ttu-id="c9691-103">Voit kopioida ja siirtää tiedostoja, kansioita ja linkkejä eri sijainteihin tiedosto kirjastossa.</span><span class="sxs-lookup"><span data-stu-id="c9691-103">You can copy and move files, folders, and links to different locations within a document library.</span></span> <span data-ttu-id="c9691-104">Voit myös kopioida kohteita eri paikkoihin.</span><span class="sxs-lookup"><span data-stu-id="c9691-104">You can also copy items across sites.</span></span> 
  
1. <span data-ttu-id="c9691-105">Selaa selaimessa tiedostot, kansiot tai linkit, jotka haluat siirtää, ja valitse sitten **Kopioi kohteeseen** tai **Siirrä kohteeseen**.</span><span class="sxs-lookup"><span data-stu-id="c9691-105">In a browser, browse to the files, folders, or links you want to move, and then click **Copy to** or **Move to**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="c9691-106">**Kopioi kohteeseen** -ja **Siirrä-** toiminnot eivät ole käytettävissä, jos käytät SharePoint Onlinen perinteistä käyttö kokemusta.</span><span class="sxs-lookup"><span data-stu-id="c9691-106">**Copy to** and **Move to** aren't available if you're using the classic experience of SharePoint Online.</span></span>
  
2. <span data-ttu-id="c9691-107">Valitse **Valitse kohde**-kohdassa sijainti, johon haluat kopioida tai siirtää kohteet, tai napsauta **Selaa sivustot** -kohtaa, niin näet luettelon kaikista alueista.</span><span class="sxs-lookup"><span data-stu-id="c9691-107">Under **Choose a destination**, select the location to which you want to copy or move the items or click **Browse sites** to see the full list of sites.</span></span>

    > [!NOTE]
    > <span data-ttu-id="c9691-108">Jos muut sivustot eivät näy, kun kopioit kohteita, kopiointia ei ole määritetty eri kohteissa.</span><span class="sxs-lookup"><span data-stu-id="c9691-108">If you don't see other sites listed when you copy items, copying across sites hasn't been configured.</span></span> <span data-ttu-id="c9691-109">Jos haluat ottaa sen käyttöön, siirry SharePoint-hallinta keskuksen asetukset-sivulle ja valitse **OK**.</span><span class="sxs-lookup"><span data-stu-id="c9691-109">To enable it, go to the settings page of the SharePoint admin center and click **OK**.</span></span>
  
    <span data-ttu-id="c9691-110">Jos haluat luoda uuden kansion, valitse sijainti kansio hierarkiassa, valitse **Uusi kansio**, Kirjoita kansiolle nimi ja Tallenna nimi valitsemalla valinta merkki.</span><span class="sxs-lookup"><span data-stu-id="c9691-110">To create a new folder, select a location in the folder hierarchy, click **New folder**, enter a name for the folder, and click the check mark to save the name.</span></span>

3. <span data-ttu-id="c9691-111">Valitse **Kopioi tähän** tai **Siirrä tähän**.</span><span class="sxs-lookup"><span data-stu-id="c9691-111">Click **Copy here** or **Move here**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="c9691-112">Voit kopioida kerralla jopa 500 Mt tiedostoja ja kansioita.</span><span class="sxs-lookup"><span data-stu-id="c9691-112">You can copy up to 500 MB of files and folders at one time.</span></span> <span data-ttu-id="c9691-113">> kun kopioit asia kirjoja, joissa on versio historia, vain uusin versio kopioidaan.</span><span class="sxs-lookup"><span data-stu-id="c9691-113">>  When you copy documents that have version history, only the latest version is copied.</span></span> <span data-ttu-id="c9691-114">Kun siirrät asia kirjoja, myös niiden historia siirretään.</span><span class="sxs-lookup"><span data-stu-id="c9691-114">When you move documents, their history is also moved.</span></span>
  
 <span data-ttu-id="c9691-115">Kun tiedosto siirretään, se näkyy edelleen lähde hakemistossa, kunnes se on siirretty kokonaan kohteeseen, ja se poistetaan.</span><span class="sxs-lookup"><span data-stu-id="c9691-115">When a file is moving, it will still appear in the source directory until its fully moved to the destination, and then it will be deleted.</span></span> <span data-ttu-id="c9691-116">Tiedosto säilyy lähde sivustot-roska korissa, kun siirto on valmis, ja sitä koskevat normaali kierrätys aikataulu, paitsi jos käyttäjä palauttaa sen roska korista.</span><span class="sxs-lookup"><span data-stu-id="c9691-116">The file will remain in the source sites recycle bin after the move is complete and be subject to the normal recycle schedule unless a user recovers it from the recycle bin.</span></span>

<span data-ttu-id="c9691-117">Lisätietoja on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="c9691-117">For more information, see:</span></span>

 - <span data-ttu-id="c9691-118">[Tiedostojen siirtäminen tai kopioiminen SharePointissa](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (Officen tuki artikkeli)</span><span class="sxs-lookup"><span data-stu-id="c9691-118">[Move or copy files in SharePoint](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (Office support article)</span></span>
 - <span data-ttu-id="c9691-119">[Tiedostojen siirtäminen mistä tahansa kansiosta](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (Microsoft Tech Community-Blogiartikkeli)</span><span class="sxs-lookup"><span data-stu-id="c9691-119">[Move files from any folder](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (Microsoft Tech Community blog article)</span></span>  