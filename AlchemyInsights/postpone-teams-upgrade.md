---
title: Teams-päivityksen lykkääminen
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
- "2737"
- "4000006"
ms.openlocfilehash: abbf696b1554743bda188704272bfd85fe6f94e2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51801228"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="1d6f1-102">Microsoft-driven Teams -päivityksen lykkääminen</span><span class="sxs-lookup"><span data-stu-id="1d6f1-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="1d6f1-103">**Tärkeää:** Voimme auttaa sinua korjaamaan ongelman käyttämällä tukidiagnostiikkaa, mutta näyttää siltä, että et käytä Uutta hallintakeskusta.</span><span class="sxs-lookup"><span data-stu-id="1d6f1-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="1d6f1-104">Jos haluat käyttää Uusi hallintakeskus -hallintakeskusta, liu'uta oikeassa yläkulmassa uutta **hallintakeskusta** oikealle.</span><span class="sxs-lookup"><span data-stu-id="1d6f1-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="1d6f1-105">Napsauta Uusi hallintakeskus -kohdassa Tarvitsetko **apua?** -pienoisohjelmaa, kirjoita "Lykkää Teams-päivitystä" ja suorita vianmääritys ohjeiden mukaan.</span><span class="sxs-lookup"><span data-stu-id="1d6f1-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="1d6f1-106">Jos olet saanut viestin Microsoftin automaattisesta päivityksestä Microsoft Teamsiin ja haluat lykätä automaattista päivitystä myöhemmäksi, yleinen järjestelmänvalvojasi voi kirjautua  [Teamsin](https://admin.teams.microsoft.com/dashboard) hallintaportaaliin ja valita Päivitä tila -painikkeen Microsoft Teams -päivityksen alla ja valita Lykkää-painikkeen. </span><span class="sxs-lookup"><span data-stu-id="1d6f1-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="1d6f1-107">Jos haluat nähdä uuden päivämäärän vuokraajan automaattiselle Microsoft Teams -päivitykselle, päivitä Teams-hallintaportaalin sivu.</span><span class="sxs-lookup"><span data-stu-id="1d6f1-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="1d6f1-108">**Huomautus:** **Lykkää-painike** on käytettävissä vain, jos olet saanut automaattista päivitystä koskevan viestikeskuksen ilmoituksen.</span><span class="sxs-lookup"><span data-stu-id="1d6f1-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="1d6f1-109">Yleiset järjestelmänvalvojat voivat myös suorittaa [Get-CsTeamsUpgradeStatus-haun](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) ja saada lisätietoja niiden nykyisestä päivitystilasta.</span><span class="sxs-lookup"><span data-stu-id="1d6f1-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
