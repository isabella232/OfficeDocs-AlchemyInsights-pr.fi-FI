---
title: OneDrive for Business Web OneDrive ohjaa Delveen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 74151ed149c57ceebc841902796189f6638795a9
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571200"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="022ae-102">Ohjattu sivulta Delve kun napsautat OneDrive</span><span class="sxs-lookup"><span data-stu-id="022ae-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="022ae-103">Katso yksityiskohtainen [vian etsintä opas](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span><span class="sxs-lookup"><span data-stu-id="022ae-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="022ae-104">Tämän ongelman ratkaisemiseksi Office 365-järjestelmänvalvojan on myönnettävä käyttäjille oikeus luoda omat sivustot-sivusto.</span><span class="sxs-lookup"><span data-stu-id="022ae-104">To resolve this problem, the Office 365 administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="022ae-105">Tämä johtuu siitä, että OneDrive for Business-sivu on luotu omat sivustot-sivulla.</span><span class="sxs-lookup"><span data-stu-id="022ae-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="022ae-106">Jos haluat myöntää tämän oikeuden, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="022ae-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="022ae-107">Valitse SharePointin hallinta keskuksessa **käyttäjä profiilit**.</span><span class="sxs-lookup"><span data-stu-id="022ae-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="022ae-108">Valitse **henkilöt** -osasta **Hallitse käyttö oikeuksia**.</span><span class="sxs-lookup"><span data-stu-id="022ae-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="022ae-109">Lisää käyttäjät, jotka edellyttävät oikeuksia omien sivustojen sivuston luomiseen.</span><span class="sxs-lookup"><span data-stu-id="022ae-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="022ae-110">Oletus asetuksena on, että tämä asetus on **kaikki ulkoiset käyttäjät lukuun ottamatta**.</span><span class="sxs-lookup"><span data-stu-id="022ae-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="022ae-111">Kun olet lisännyt käyttäjän, käyttäjät tai ryhmän, varmista, että lisätty käyttäjä, käyttäjät tai ryhmä on valittuna, vieritä **käyttö oikeudet** -osioon ja valitse Luo henkilökohtainen sivusto-kohdan vieressä oleva valinta ruutu **(tarvitaan henkilökohtaiseen tallennukseen, uutis syötteeseen ja seuratun sisällön käyttöön)**.</span><span class="sxs-lookup"><span data-stu-id="022ae-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="022ae-112">Valitse **OK**ja sitten käyttäjä Selaa OneDrive-sivulle ja luo sivusto.</span><span class="sxs-lookup"><span data-stu-id="022ae-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
