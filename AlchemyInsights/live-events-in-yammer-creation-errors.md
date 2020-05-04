---
title: Yammerin livetapahtumien luomisvirheet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002495"
- "5112"
ms.openlocfilehash: 35cddfee1a78fd6e1e502871bd5b56d786bf300a
ms.sourcegitcommit: fbaa2ce2cfb4d56d8c4cf2fa2d95489bdfcb7ff0
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/30/2020
ms.locfileid: "43947827"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="97a2d-102">Yammerin livetapahtumien luomisvirheet</span><span class="sxs-lookup"><span data-stu-id="97a2d-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="97a2d-103">**Yammer-livetapahtuman luominen**</span><span class="sxs-lookup"><span data-stu-id="97a2d-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="97a2d-104">Yammerissa näkyy aina livetapahtuman luomisvalinta.</span><span class="sxs-lookup"><span data-stu-id="97a2d-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="97a2d-105">Joissakin tapauksissa käyttäjä ei ehkä täytä livetapahtuman luomisen edellytyksiä, ja hän näkee virheviestin yrittäessään luoda livetapahtuman.</span><span class="sxs-lookup"><span data-stu-id="97a2d-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="97a2d-106">Alla olevissa kohdissa eritellään tämän ongelman yleiset syyt ja tarjotaan ratkaisutavat loppukäyttäjille.</span><span class="sxs-lookup"><span data-stu-id="97a2d-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="97a2d-107">**Kuka voi luoda livetapahtumia**</span><span class="sxs-lookup"><span data-stu-id="97a2d-107">**Who can create live events**</span></span>
- <span data-ttu-id="97a2d-108">Tarvitset Office 365 Enterprise E1-, E3- tai E5-käyttöoikeuden tai Office 365 A3- tai A5-käyttöoikeuden.</span><span class="sxs-lookup"><span data-stu-id="97a2d-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="97a2d-109">Tarvitset oikeuden luoda livetapahtumia Microsoft Teams -hallintakeskuksessa.</span><span class="sxs-lookup"><span data-stu-id="97a2d-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="97a2d-110">Tarvitset oikeuden luoda livetapahtumia Microsoft Streamissa (tapahtumat, jotka tuotetaan ulkoisella lähetyssovelluksella tai -laitteella).</span><span class="sxs-lookup"><span data-stu-id="97a2d-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="97a2d-111">Tarvitset organisaation täyden jäsenyyden (et voi olla vieras tai toisesta organisaatiosta).</span><span class="sxs-lookup"><span data-stu-id="97a2d-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="97a2d-112">Yksityisten kokousten järjestämisen, näytön jakamisen ja IP-kuvayhteyden jakamisen täytyy olla käytössä Teamsin kokouskäytännössä.</span><span class="sxs-lookup"><span data-stu-id="97a2d-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="97a2d-113">**Livetapahtuman luomiskäytännöt**</span><span class="sxs-lookup"><span data-stu-id="97a2d-113">**Live event creation policies**</span></span>

<span data-ttu-id="97a2d-114">Yammer noudattaa Streamin Office 365 -vuokraajassa määritettyjä livetapahtumakäytäntöjä.</span><span class="sxs-lookup"><span data-stu-id="97a2d-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="97a2d-115">Kaikki organisaation jäsenet voivat oletusarvoisesti luoda livetapahtumia.</span><span class="sxs-lookup"><span data-stu-id="97a2d-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="97a2d-116">Järjestelmänvalvojat voivat [muuttaa tätä asetusta, mikä saattaa estää käyttäjiä luomasta livetapahtumia](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span><span class="sxs-lookup"><span data-stu-id="97a2d-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="97a2d-117">On tärkeää tarkistaa, että käyttäjillä on oikeus luoda livetapahtumia, jos he saavat käytäntövirheilmoituksen.</span><span class="sxs-lookup"><span data-stu-id="97a2d-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>
