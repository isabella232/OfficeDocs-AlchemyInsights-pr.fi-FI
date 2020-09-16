---
title: Teamsin Salli tai Poista käytöstä IP-video
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002537"
- "5617"
ms.openlocfilehash: cf2d67170f846db1d5d2f1ca8c8b50902e200e45
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670181"
---
# <a name="teams-allow-or-disable-ip-video"></a><span data-ttu-id="ae48d-102">Teamsin Salli tai Poista käytöstä IP-video</span><span class="sxs-lookup"><span data-stu-id="ae48d-102">Teams allow or disable IP video</span></span>

<span data-ttu-id="ae48d-103">**Kokous käytäntöjen muuttaminen tai luominen**</span><span class="sxs-lookup"><span data-stu-id="ae48d-103">**Change or create a meeting policy**</span></span>

<span data-ttu-id="ae48d-104">Jos haluat muuttaa tai luoda Kokous käytäntöä, siirry **Microsoft teamsin hallinta keskukseen > koko ukseen > Kokous käytännöt**.</span><span class="sxs-lookup"><span data-stu-id="ae48d-104">To change or create a meeting policy, go to the **Microsoft Teams admin center > Meetings > Meeting policies**.</span></span> <span data-ttu-id="ae48d-105">Valitse käytäntö luettelosta tai valitse **Lisää**.</span><span class="sxs-lookup"><span data-stu-id="ae48d-105">Select a policy from the list or click **Add**.</span></span> <span data-ttu-id="ae48d-106">Jos luot uutta käytäntöä, kirjoita nimi ja kuvaus.</span><span class="sxs-lookup"><span data-stu-id="ae48d-106">If you're creating a new policy, add a name and description.</span></span> <span data-ttu-id="ae48d-107">Nimi ei voi sisältää erikoismerkkejä, ja sen pituus voi olla enintään 64 merkkiä.</span><span class="sxs-lookup"><span data-stu-id="ae48d-107">The name can't contain special characters or be longer than 64 characters.</span></span> <span data-ttu-id="ae48d-108">Valitse asetukset ja valitse sitten **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="ae48d-108">Choose your settings, and then click **Save**.</span></span>

<span data-ttu-id="ae48d-109">Oletetaan esimerkiksi, että sinulla on useita käyttäjiä ja haluat rajoittaa koko uksen edellyttämään kaistan leveyden määrää.</span><span class="sxs-lookup"><span data-stu-id="ae48d-109">For example, say you have many users and you want to limit the amount of bandwidth that their meeting would require.</span></span> <span data-ttu-id="ae48d-110">Tällöin voit luoda uuden käytännön nimeltä Rajoitettu kaistanleveys ja ottaa pois käytöstä seuraavat asetukset:</span><span class="sxs-lookup"><span data-stu-id="ae48d-110">You would create a new custom policy named "Limited bandwidth" and disable the following settings:</span></span>

<span data-ttu-id="ae48d-111">Kohdassa **Ääni ja video**:</span><span class="sxs-lookup"><span data-stu-id="ae48d-111">Under **Audio & video**:</span></span>

- <span data-ttu-id="ae48d-112">Poista käytöstä Salli pilvitallennus.</span><span class="sxs-lookup"><span data-stu-id="ae48d-112">Turn off Allow cloud recording.</span></span>
- <span data-ttu-id="ae48d-113">Poista käytöstä Salli IP-video.</span><span class="sxs-lookup"><span data-stu-id="ae48d-113">Turn off Allow IP video.</span></span>

<span data-ttu-id="ae48d-114">Määritä sitten käytäntö käyttäjille.</span><span class="sxs-lookup"><span data-stu-id="ae48d-114">Then assign the policy to the users.</span></span>

<span data-ttu-id="ae48d-115">**Kokouskäytännön määrittäminen käyttäjille**</span><span class="sxs-lookup"><span data-stu-id="ae48d-115">**Assign a meeting policy to users**</span></span>

1. <span data-ttu-id="ae48d-116">Siirry Microsoft Teams -hallintakeskuksen vasemmanpuoleisessa siirtymisvalikossa kohtaan **Käyttäjät** ja valitse käyttäjä.</span><span class="sxs-lookup"><span data-stu-id="ae48d-116">In the left navigation of the Microsoft Teams admin center, go to **Users**, and then click the user.</span></span>
2. <span data-ttu-id="ae48d-117">Valitse käyttäjä napsauttamalla käyttäjänimen vasemmalta puolelta ja valitse sitten **Muokkaa asetuksia**.</span><span class="sxs-lookup"><span data-stu-id="ae48d-117">Select the user by clicking to the left of the user name, and then click **Edit settings**.</span></span>
3. <span data-ttu-id="ae48d-118">Valitse **koko uksen käytännöt**-kohdassa se, jonka haluat määrittää, ja valitse sitten **Käytä**.</span><span class="sxs-lookup"><span data-stu-id="ae48d-118">Under **Meeting policy**, select the policy you want to assign and then click **Apply**.</span></span>

<span data-ttu-id="ae48d-119">Lisä tietoja on kohdassa [Kokous käytäntöjen hallinta teamsissa](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="ae48d-119">For more information, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>
