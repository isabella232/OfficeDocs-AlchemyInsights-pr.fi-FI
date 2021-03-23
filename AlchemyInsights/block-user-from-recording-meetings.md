---
title: Estä käyttäjää kokousten tallentamisesta
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "9325"
ms.openlocfilehash: 3f633ee1fb3329b6fc634acabbc824af1eccfb33
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035365"
---
# <a name="block-user-from-recording-meetings"></a><span data-ttu-id="a7496-102">Estä käyttäjää kokousten tallentamisesta</span><span class="sxs-lookup"><span data-stu-id="a7496-102">Block User From Recording Meetings</span></span>

<span data-ttu-id="a7496-103">Jos haluat estää **tai estää tiettyjä käyttäjiä** nauhoittamasta Teams-kokouksia, voit tehdä sen Teamsin kokouskäytäntöasetusten kautta.</span><span class="sxs-lookup"><span data-stu-id="a7496-103">If you need to **prevent or block** specific users from recording Teams Meetings, you can do so via Teams Meeting Policy settings.</span></span> <span data-ttu-id="a7496-104">Poista Microsoft Teams -hallintakeskuksessa  käyttäjälle määritetyn kokouskäytännön Salli pilvitallennus -asetus käytöstä.</span><span class="sxs-lookup"><span data-stu-id="a7496-104">In the Microsoft Teams admin center, turn off the **Allow cloud recording** setting in the meeting policy assigned to that user.</span></span> <span data-ttu-id="a7496-105">Lisätietoja on ohjeaiheessa [Kokouskäytäntöjen hallinta Teamsissa.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording)</span><span class="sxs-lookup"><span data-stu-id="a7496-105">To learn more, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).</span></span>

<span data-ttu-id="a7496-106">Jos haluat tarkistaa, onko tietty käyttäjä sallittu tai ei voi tallentaa Teams-kokouksia, käytä tuen vianmääritystä.</span><span class="sxs-lookup"><span data-stu-id="a7496-106">To validate if a specific user is allowed or not to record Teams Meetings, use the support diagnostic.</span></span> <span data-ttu-id="a7496-107">Suorita uusi tukikysely ja kirjoita **Diag:** Kokoustallenne – vianmääritys tarkistaa määritetyn käyttäjän käytäntöasetukset ja määrittää hänen käytäntöasetukset.</span><span class="sxs-lookup"><span data-stu-id="a7496-107">Run a new support query and type in **Diag: Meeting Recording** - the diagnostic will check policy settings for the specified user and determine their policy settings.</span></span> <span data-ttu-id="a7496-108">Muista, että uusien käytäntöasetusten voimaan saaminen voi kestää muutaman tunnin, joten jos olet juuri tehnyt muutoksen, odota muutama tunti ennen vianmääritystä uudelleen.</span><span class="sxs-lookup"><span data-stu-id="a7496-108">Remember, it can take a couple of hours for new policy settings to take effect, so if you have just made a change, wait a few hours before running the diagnostic again.</span></span>

<span data-ttu-id="a7496-109">Lisätietoja on kohdassa [Pilvitallenteen käyttöönottaminen tai käytöstä poistaminen.](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording)</span><span class="sxs-lookup"><span data-stu-id="a7496-109">For more information, review [Turn on or turn off cloud recording](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording).</span></span>
