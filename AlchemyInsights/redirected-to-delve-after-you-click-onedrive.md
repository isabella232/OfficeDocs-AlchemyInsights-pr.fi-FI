---
title: OneDrive for Business Web OneDrive ohjaa uudelleen Delveen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51799986"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="a0a19-102">Uudelleenohjattu Delveen, kun valitset OneDrive</span><span class="sxs-lookup"><span data-stu-id="a0a19-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="a0a19-103">Katso yksityiskohtainen [vianmääritysopas](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span><span class="sxs-lookup"><span data-stu-id="a0a19-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="a0a19-104">Järjestelmänvalvojan on myönnettävä käyttäjille oikeus luoda omat sivustot -sivustonsa, jotta he voivat ratkaista ongelman.</span><span class="sxs-lookup"><span data-stu-id="a0a19-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="a0a19-105">Tämä johtuu siitä, että OneDrive for Business -sivu luodaan Omat sivustot -sivulle.</span><span class="sxs-lookup"><span data-stu-id="a0a19-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="a0a19-106">Myönnä tämä oikeus seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="a0a19-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="a0a19-107">Valitse SharePoint-hallintakeskuksessa **käyttäjäprofiilit**.</span><span class="sxs-lookup"><span data-stu-id="a0a19-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="a0a19-108">Valitse **Henkilöt-osassa** **Käyttöoikeuksien hallinta**.</span><span class="sxs-lookup"><span data-stu-id="a0a19-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="a0a19-109">Voit lisätä käyttäjiä, jotka tarvitsevat omat sivustot -sivuston luontioikeudet.</span><span class="sxs-lookup"><span data-stu-id="a0a19-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="a0a19-110">Asetuksena on oletusarvoisesti Kaikki paitsi **ulkoiset käyttäjät.**</span><span class="sxs-lookup"><span data-stu-id="a0a19-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="a0a19-111">Kun olet lisännyt käyttäjän, käyttäjät tai ryhmän, varmista, että lisätty käyttäjä, käyttäjät tai  ryhmä on valittuna, vieritä Käyttöoikeudet-osioon ja valitse sitten Luo oma sivusto -kohdan vieressä olevaa valintaruutua (tarvitaan henkilökohtaiseen tallennustilaan, uutissyötteen ja seuratulle **sisällölle).**</span><span class="sxs-lookup"><span data-stu-id="a0a19-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="a0a19-112">Valitse **OK** ja valitse sitten käyttäjä selaamalla OneDrive-sivulle ja luomaan sivusto.</span><span class="sxs-lookup"><span data-stu-id="a0a19-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
