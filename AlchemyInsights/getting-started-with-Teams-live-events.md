---
title: Teamsin livetapahtumien käytön aloittaminen
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
- "9000208"
- "3436"
ms.openlocfilehash: a10f756fc69a7a135446d8d3bcec1f5e951627d8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811957"
---
# <a name="getting-started-with-teams-live-events"></a><span data-ttu-id="53612-102">Teamsin livetapahtumien käytön aloittaminen</span><span class="sxs-lookup"><span data-stu-id="53612-102">Getting started with Teams live events</span></span>

<span data-ttu-id="53612-103">Microsoft Teamsin livetapahtumat ovat Teams-kokousten laajennuksia, joiden avulla voit tuottaa tapahtumia suoratoistettavaksi suurelle yleisölle.</span><span class="sxs-lookup"><span data-stu-id="53612-103">Microsoft Teams live events are an extension of Teams meetings that enable you to schedule and produce events that stream to large online audiences.</span></span>

<span data-ttu-id="53612-104">Tarvitset livetapahtuman luomiseen seuraavat:</span><span class="sxs-lookup"><span data-stu-id="53612-104">To create a live event, you will need the following:</span></span>

- <span data-ttu-id="53612-105">Varmista ensin, että Teams live -tapahtumat [ovat käytettävissä maassasi ja alueellasi;](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability) Live-tapahtumia ei tueta vielä joissakin maissa.</span><span class="sxs-lookup"><span data-stu-id="53612-105">First, confirm that Teams Live Events are [available in your Country and Region](https://docs.microsoft.com/microsoftteams/teams-live-events/plan-for-teams-live-events#regional-availability); Live Events are not yet supported in some countries.</span></span>  <span data-ttu-id="53612-106">Jos olet määrittänyt käyttöoikeuksia ja määrittänyt käytäntöjä, mutta et silti voi luoda Teams Live -tapahtumaa, olet todennäköisesti maassa tai alueella, jossa Live-tapahtumat eivät ole vielä käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="53612-106">If you’ve assigned licenses and set policies, but still cannot create a Teams Live Event, it is likely you are in a Country or Region where Live Events is not yet available.</span></span>

- <span data-ttu-id="53612-107">Tarvitset jonkin seuraavista käyttöoikeuksista: [Office 365 Enterprise E1, E3 tai E5 tai Office 365 A3 tai A5](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span><span class="sxs-lookup"><span data-stu-id="53612-107">An [Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#step-2-get-and-assign-licenses).</span></span> <span data-ttu-id="53612-108">**Huomautus**: Koska Teamsin käyttö on kasvanut merkittävästi viime aikoina, käyttöoikeuden käyttäjälle määrittämisestä saattaa kulua jopa 24 tuntia, ennen kuin kyseinen käyttäjä on täysin käyttövalmis.</span><span class="sxs-lookup"><span data-stu-id="53612-108">**Note**: Due to a recent increase in Teams usage, when you assign a Teams license to a user, it may take around 24 hours before they'll be fully set up.</span></span> <span data-ttu-id="53612-109">Ennen tätä et voi määrittää kyseiselle käyttäjälle Teams-käytäntöjä eikä hän ehkä voi käyttää joitain Teamsin toimintoja, esimerkiksi puheluita tai puhelinneuvotteluita.</span><span class="sxs-lookup"><span data-stu-id="53612-109">Until then, you won't be able to assign Teams policies to them, and they might not have access to some Teams features like calling and audio conferencing.</span></span>

- <span data-ttu-id="53612-110">Tarvitset [oikeuden luoda livetapahtumia Microsoft Teamsin hallintakeskuksessa](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span><span class="sxs-lookup"><span data-stu-id="53612-110">Permission to [create live events in Microsoft Teams admin center](https://docs.microsoft.com/microsoftteams/teams-live-events/set-up-for-teams-live-events#create-or-edit-a-live-events-policy).</span></span>

- <span data-ttu-id="53612-111">Tarvitset [oikeuden luoda livetapahtumia Microsoft Streamissa](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (tapahtumat, jotka tuotetaan ulkoisella lähetyssovelluksella tai -laitteella).</span><span class="sxs-lookup"><span data-stu-id="53612-111">Permission to [create live events in Microsoft Stream](https://docs.microsoft.com/microsoftteams/teams-live-events/what-are-teams-live-events) (for events produced using an external broadcasting app or device).</span></span>

- <span data-ttu-id="53612-112">Tarvitset täyden tiimijäsenyyden organisaatiossa (et voi olla vieras tai toisesta organisaatiosta).</span><span class="sxs-lookup"><span data-stu-id="53612-112">Full team membership in the org (can't be a guest or from another org).</span></span>
<span data-ttu-id="53612-113">Yksityisten kokousten järjestämisen, näytön jakamisen ja IP-kuvayhteyden jakamisen täytyy olla käytössä Teamsin kokouskäytännössä.</span><span class="sxs-lookup"><span data-stu-id="53612-113">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

- <span data-ttu-id="53612-114">Tutustu Teamsin livetapahtumien [parhaisiin käytäntöihin](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42).</span><span class="sxs-lookup"><span data-stu-id="53612-114">[Best practices](https://support.office.com/article/Best-practices-for-producing-a-Teams-live-event-e500370e-4dd1-4187-8b48-af10ef02cf42) for Teams Live Events.</span></span>

<span data-ttu-id="53612-115">Saat lisätietoja ohjeartikkelista [Microsoft Teamsin live-tapahtumien käytön aloittaminen](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span><span class="sxs-lookup"><span data-stu-id="53612-115">For more information, please see [Get started with Microsoft Teams live events](https://support.office.com/article/get-started-with-microsoft-teams-live-events-d077fec2-a058-483e-9ab5-1494afda578a).</span></span>