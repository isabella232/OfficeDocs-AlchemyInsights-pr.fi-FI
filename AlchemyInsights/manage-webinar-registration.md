---
title: Verkkoseinaarin rekisteröinnin hallinta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793708"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="0fe09-102">Verkkoseinaarin rekisteröinnin hallinta</span><span class="sxs-lookup"><span data-stu-id="0fe09-102">Manage webinar registration</span></span>

<span data-ttu-id="0fe09-103">Voit hallita sitä, kuka voi rekisteröityä Teams Webinaarit-Teams PowerShell-komennoilla.</span><span class="sxs-lookup"><span data-stu-id="0fe09-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="0fe09-104">Jos haluat asentaa Teams PowerShellin, katso [Teams PowerShelliä.](/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="0fe09-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="0fe09-105">*Oletusarvoisesti WhoCanRegister* on käytössä ja sen asetuksena **on EveryoneInCompany.**</span><span class="sxs-lookup"><span data-stu-id="0fe09-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="0fe09-106">Jotta kuka tahansa, anonyymit käyttäjät mukaan lukien, voi  rekisteröityä, sinun on määritettävä kokouskäytännön arvoksi Kaikki PowerShell-komennolla:</span><span class="sxs-lookup"><span data-stu-id="0fe09-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="0fe09-107">**Huomautus:** Jos anonyymi liittyminen on poistettu käytöstä kokousasetuksissa, anonyymit käyttäjät eivät voi liittyä webinaariin.</span><span class="sxs-lookup"><span data-stu-id="0fe09-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="0fe09-108">Lisätietoja ja tämän asetuksen käyttöönotto on kohdassa [Kokousasetusten hallinta Microsoft Teams.](/microsoftteams/meeting-settings-in-teams)</span><span class="sxs-lookup"><span data-stu-id="0fe09-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="0fe09-109">Jos haluat poistaa kokouksen rekisteröinnin käytöstä, määritä *AllowMeetingRegistration-asetuksen arvoksi* **Epätosi.**</span><span class="sxs-lookup"><span data-stu-id="0fe09-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="0fe09-110">Lisätietoja sen määrittämisestä, kuka voi rekisteröityä webinaariin, on kohdassa Määritä, [kuka voi rekisteröityä webinaariin.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="0fe09-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="0fe09-111">Lisätietoja Microsoft-luetteloiden asetuksista on artikkelissa [Microsoft-luetteloiden asetusten hallinta.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="0fe09-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
