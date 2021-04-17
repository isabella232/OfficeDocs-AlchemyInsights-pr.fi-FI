---
title: Teams sallii tai poistaa käytöstä IP-videon
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: 059d7a1ad619e25f14bc6f561693b6fe24355132
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826340"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="d7725-102">Teams sallii tai poistaa käytöstä IP-videon</span><span class="sxs-lookup"><span data-stu-id="d7725-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="d7725-103">**Kokouskäytännön muuttaminen tai luominen**</span><span class="sxs-lookup"><span data-stu-id="d7725-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="d7725-104">Jos haluat muuttaa tai luoda kokouskäytännön, siirry **Microsoft Teams -hallintakeskukseen, jossa > kokouskäytäntöjä > kokouskäytäntöjä.**</span><span class="sxs-lookup"><span data-stu-id="d7725-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="d7725-105">Valitse käytäntö luettelosta tai valitse **Lisää**.</span><span class="sxs-lookup"><span data-stu-id="d7725-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="d7725-106">Jos luot uutta käytäntöä, kirjoita nimi ja kuvaus.</span><span class="sxs-lookup"><span data-stu-id="d7725-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="d7725-107">Nimi ei voi sisältää erikoismerkkejä, ja sen pituus voi olla enintään 64 merkkiä.</span><span class="sxs-lookup"><span data-stu-id="d7725-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="d7725-108">Valitse asetukset ja valitse sitten **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="d7725-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="d7725-109">Oletetaan esimerkiksi, että sinulla on useita käyttäjiä ja haluat rajoittaa kokousten edellytettävän kaistanleveyden määrää.</span><span class="sxs-lookup"><span data-stu-id="d7725-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="d7725-110">Tällöin voit luoda uuden käytännön nimeltä Rajoitettu kaistanleveys ja ottaa pois käytöstä seuraavat asetukset:</span><span class="sxs-lookup"><span data-stu-id="d7725-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="d7725-111">Kohdassa **Ääni ja video**:</span><span class="sxs-lookup"><span data-stu-id="d7725-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="d7725-112">Poista käytöstä Salli pilvitallennus.</span><span class="sxs-lookup"><span data-stu-id="d7725-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="d7725-113">Poista käytöstä Salli IP-video.</span><span class="sxs-lookup"><span data-stu-id="d7725-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="d7725-114">Määritä sitten käytäntö käyttäjille.</span><span class="sxs-lookup"><span data-stu-id="d7725-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="d7725-115">**Kokouskäytännön määrittäminen käyttäjille**</span><span class="sxs-lookup"><span data-stu-id="d7725-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="d7725-116">Siirry Microsoft Teams -hallintakeskuksen vasemmanpuoleisessa siirtymisvalikossa kohtaan **Käyttäjät** ja valitse käyttäjä.</span><span class="sxs-lookup"><span data-stu-id="d7725-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="d7725-117">Valitse käyttäjä napsauttamalla käyttäjänimen vasemmalta puolelta ja valitse sitten **Muokkaa asetuksia**.</span><span class="sxs-lookup"><span data-stu-id="d7725-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="d7725-118">Valitse **Kokouskäytäntö-kohdassa** käytäntö, jonka haluat määrittää, ja valitse sitten **Käytä**.</span><span class="sxs-lookup"><span data-stu-id="d7725-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="d7725-119">Lisätietoja on kohdassa [Kokouskäytäntöjen hallinta Teamsissa.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="d7725-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
