---
title: Yammerin kuvien lataamiseen liittyvien ongelmien vianmääritys
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6000"
- "9003112"
ms.openlocfilehash: 93894eaa5818b591acd1c7b9a90bc1cabbe00450
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148227"
---
# <a name="troubleshoot-image-loading-issues-in-yammer"></a><span data-ttu-id="aa9a7-102">Yammerin kuvien lataamiseen liittyvien ongelmien vianmääritys</span><span class="sxs-lookup"><span data-stu-id="aa9a7-102">Troubleshoot image loading issues in Yammer</span></span>

<span data-ttu-id="aa9a7-103">Kun Yammerin valokuvien ja tiedostojen esikatseluissa ilmenee ongelmia, tee vianmääritys tarkistamalla, ilmeneekö ongelma kaikille käyttäjille, esiintyykö ongelma mobiililaitteissa ja onko se toistettavissa liitetiedoston lataamisen yhteydessä.</span><span class="sxs-lookup"><span data-stu-id="aa9a7-103">When issues occur with photos and file previews in Yammer, troubleshoot by checking whether the issue occurs for all users, whether it occurs on mobile devices, and if it is reproducible when uploading the attachment.</span></span>  

<span data-ttu-id="aa9a7-104">**Profiilikuvan ongelmat**</span><span class="sxs-lookup"><span data-stu-id="aa9a7-104">**Profile photo issues**</span></span>  

<span data-ttu-id="aa9a7-105">Jos loppukäyttäjät kirjautuvat Yammerin kautta Microsoft 365:n kautta, heidän on muutettava profiiliaan, mukaan lukien profiilikuvansa.</span><span class="sxs-lookup"><span data-stu-id="aa9a7-105">If end users sign into Yammer via Microsoft 365, they must change their profile, including their profile photo.</span></span> <span data-ttu-id="aa9a7-106">Jos käyttäjät eivät saa tehdä profiilipäivityksiä, järjestelmänvalvoja voi tehdä päivityksen käyttäjälle.</span><span class="sxs-lookup"><span data-stu-id="aa9a7-106">If users are not permitted to make profile updates, an admin can make the update for the user.</span></span> <span data-ttu-id="aa9a7-107">Lisätietoja on [ohjeaiheessa Profiilin tarkasteleminen ja päivittäminen Office Delvessä](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span><span class="sxs-lookup"><span data-stu-id="aa9a7-107">For more info, see [View and update your profile in Office Delve](https://support.microsoft.com/office/view-and-update-your-profile-in-office-delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>

<span data-ttu-id="aa9a7-108">Lisätietoja profiilin muokkaamisesta, mukaan lukien profiilikuvat, [on ohjeaiheessa Yammer-profiilin ja -asetusten muuttaminen](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span><span class="sxs-lookup"><span data-stu-id="aa9a7-108">For info about profile editing, including profile photos, see [Change my Yammer profile and settings](https://support.microsoft.com/office/classic-yammer-change-my-yammer-profile-and-settings-a3aeca0e-de34-4897-9b59-de6516542851).</span></span> 

<span data-ttu-id="aa9a7-109">Päivitetyt profiilikuvat synkronoidaan eri tavalla kuin profiilimääritteet.</span><span class="sxs-lookup"><span data-stu-id="aa9a7-109">Updated profile photos are synced differently than profile attributes.</span></span> <span data-ttu-id="aa9a7-110">Käyttäjien on kirjauduttava sisään, jotta he voivat synkronoida profiilikuvansa.</span><span class="sxs-lookup"><span data-stu-id="aa9a7-110">Users must sign in to initiate a sync of their profile photo.</span></span> <span data-ttu-id="aa9a7-111">Lisätietoja on kohdassa [Ovat office 365:stä Yammeriin päivitettyjä käyttäjäprofiilikuvia](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span><span class="sxs-lookup"><span data-stu-id="aa9a7-111">For info, see [are user profile pictures updated from Office 365 to Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle#q-are-user-profile-pictures-updated-from-office-365-to-yammer).</span></span>

<span data-ttu-id="aa9a7-112">Lisätietoja Yammerin käyttäjän elinkaaresta on [ohjeaiheessa Yammerin käyttäjien hallinta koko niiden elinkaaren ajan Office 365:stä](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span><span class="sxs-lookup"><span data-stu-id="aa9a7-112">For info about the user lifecycle for Yammer, see [Manage Yammer users across their lifecycle from Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-users-across-their-lifecycle).</span></span>  

<span data-ttu-id="aa9a7-113">Lisätietoja profiilikuvan synkronoinnin toiminnasta Microsoft 365:ssä on [ohjeaiheessa Tietoja profiilikuvan synkronoinnista Microsoft 365:ssä](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span><span class="sxs-lookup"><span data-stu-id="aa9a7-113">For details on how profile picture sync works in Microsoft 365, see [Information about profile picture synchronization in Microsoft 365](https://support.microsoft.com/office/information-about-profile-picture-synchronization-in-microsoft-365-20594d76-d054-4af4-a660-401133e3d48a).</span></span>  

<span data-ttu-id="aa9a7-114">**Asiakirjan esikatselut ja pikkukuvaongelmat**</span><span class="sxs-lookup"><span data-stu-id="aa9a7-114">**Document previews and image thumbnail issues**</span></span>  

<span data-ttu-id="aa9a7-115">Kun tiedostot tai kuvat on lähetetty Yammeriin, esikatselut eivät välttämättä näy, koska:</span><span class="sxs-lookup"><span data-stu-id="aa9a7-115">When files or images are posted to Yammer, previews might not appear because:</span></span> 

- <span data-ttu-id="aa9a7-116">Tiedosto on vioittunut, eikä sitä voi käsitellä.</span><span class="sxs-lookup"><span data-stu-id="aa9a7-116">The file is corrupt and cannot be processed.</span></span>
- <span data-ttu-id="aa9a7-117">Tiedostoa ei ole äskettäin ladattu SharePoint Onlineen, tai Yammerilla on virheellisiä metatietoja muista syistä.</span><span class="sxs-lookup"><span data-stu-id="aa9a7-117">The file has not been recently uploaded to SharePoint Online, or Yammer has invalid metadata for other reasons.</span></span>
- <span data-ttu-id="aa9a7-118">Esikatselukuvien lataamiseen tarvittavat URL-osoitteet on estetty.</span><span class="sxs-lookup"><span data-stu-id="aa9a7-118">URLs required for loading the preview images are blocked.</span></span>
- <span data-ttu-id="aa9a7-119">Käyttäjä poisti tiedoston esikatselun ennen kirjausta.</span><span class="sxs-lookup"><span data-stu-id="aa9a7-119">The file preview was removed by the user before posting.</span></span>
- <span data-ttu-id="aa9a7-120">Palveluongelma esti esikatselun luomisen.</span><span class="sxs-lookup"><span data-stu-id="aa9a7-120">A service issue prevented a preview being generated.</span></span>

<span data-ttu-id="aa9a7-121">**Huomautus** Linkkien ja tiedostojen lataamisen esikatselut saattavat toimia eri tavalla.</span><span class="sxs-lookup"><span data-stu-id="aa9a7-121">**Note** Previews for links and file uploads might behave differently.</span></span> <span data-ttu-id="aa9a7-122">Linkit Internetissä oleviin tiedostoihin tai linkkejä, jotka edellyttävät lisätodennusta, eivät ehkä näy oikein.</span><span class="sxs-lookup"><span data-stu-id="aa9a7-122">Links to files on the internet or links that require additional authentication might not display correctly.</span></span>

<span data-ttu-id="aa9a7-123">Lisätietoja on [ohjeaiheessa Tiedoston tai kuvan liittäminen Yammer-viestiin](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span><span class="sxs-lookup"><span data-stu-id="aa9a7-123">For more info, see [Attach a file or image to a Yammer message](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-message-f576d4d1-ad66-4ce4-9c43-46cf75978dbf).</span></span> 