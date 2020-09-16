---
title: OneDrive for Business Web OneDrive ohjaa Delvessä
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: faa2cf25270a3b74a12aeb63d23ce98b51e13cb6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776376"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="0c769-102">Uudelleenohjataan Delveen, kun napsautat OneDrive</span><span class="sxs-lookup"><span data-stu-id="0c769-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="0c769-103">Tutustu yksityiskohtaiseen [vian määritys oppaaseen](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span><span class="sxs-lookup"><span data-stu-id="0c769-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="0c769-104">Tämän ongelman ratkaisemiseksi hallinnoijan on annettava käyttäjille oikeus luoda omat sivustot-sivustonsa.</span><span class="sxs-lookup"><span data-stu-id="0c769-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="0c769-105">Tämä johtuu siitä, että OneDrive for Business-sivu luodaan omiin sivustoon.</span><span class="sxs-lookup"><span data-stu-id="0c769-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="0c769-106">Jos haluat myöntää tämän oikeuden, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="0c769-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="0c769-107">Valitse SharePoint-hallinta keskuksessa **käyttäjä profiilit**.</span><span class="sxs-lookup"><span data-stu-id="0c769-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="0c769-108">Valitse **henkilöt** -osiossa **Hallitse käyttö oikeuksia**.</span><span class="sxs-lookup"><span data-stu-id="0c769-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="0c769-109">Lisää käyttäjät, jotka tarvitsevat käyttö oikeuksia oman sivustonsa luomiseen.</span><span class="sxs-lookup"><span data-stu-id="0c769-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="0c769-110">Oletusarvoisesti tämä asetus on **Kaikki paitsi ulkoiset käyttäjät**.</span><span class="sxs-lookup"><span data-stu-id="0c769-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="0c769-111">Kun olet lisännyt käyttäjän, käyttäjät tai ryhmän, varmista, että lisätty käyttäjä, käyttäjät tai ryhmä on valittuna, vieritä **käyttö oikeudet** -osioon ja valitse sitten Luo oma sivusto-kohdan vieressä oleva valinta ruutu **(pakollinen henkilökohtaiseen tallennus tilaan, uutis syötteeseen ja seurattujen sisältöjen käyttöön)**.</span><span class="sxs-lookup"><span data-stu-id="0c769-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="0c769-112">Valitse **OK**ja valitse sitten käyttäjä, joka luo sivuston selaamalla OneDrive-sivulle.</span><span class="sxs-lookup"><span data-stu-id="0c769-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
