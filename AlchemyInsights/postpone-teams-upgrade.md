---
title: Ajoita teamsin päivitys
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
- "2737"
- "4000006"
ms.openlocfilehash: ae0611df247790200d0192e018ff5f0128f23cb4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741768"
---
# <a name="how-to-postpone-the-microsoft-driven-teams-upgrade"></a><span data-ttu-id="410fe-102">Microsoft-odotuksiin perustuvien tiimien päivityksen lykkääminen</span><span class="sxs-lookup"><span data-stu-id="410fe-102">How to postpone the Microsoft-driven Teams upgrade</span></span>

<span data-ttu-id="410fe-103">**Tärkeää**: voimme auttaa korjaamaan ongelman käyttämällä tuki diagnostiikkaa, mutta näyttää siltä, ettet käytä uutta hallinta keskusta.</span><span class="sxs-lookup"><span data-stu-id="410fe-103">**Important**: We can help fix this for you using a support diagnostic, but it looks like you are not using the New Admin Center.</span></span> <span data-ttu-id="410fe-104">Jos haluat käyttää uutta hallinta keskusta, liu'uta oikeassa yläkulmassa olevaa vaihto painiketta, jossa lukee **Uusi hallinta keskus** oikealle.</span><span class="sxs-lookup"><span data-stu-id="410fe-104">To use the New Admin Center, slide the toggle in the top right that says **new admin center** to the right.</span></span> <span data-ttu-id="410fe-105">Kun käytät uutta hallinta keskusta, napsauta **Tarvitsetko apua?** -widgetiä, kirjoita "Lyme teamsin päivitys" ja Suorita diagnostiikka noudattamalla kehotteita.</span><span class="sxs-lookup"><span data-stu-id="410fe-105">Using the New Admin Center, click the **Need Help?** widget, type "Postpone Teams Upgrade", then follow the prompts to run the diagnostic.</span></span>

<span data-ttu-id="410fe-106">Jos sait tiedon annon Microsoft-pohjaista, Skype for Businessin automatisoidusta päivityksestä Microsoft Teamsiin ja haluat siirtää automatisoidun päivityksen myöhempään ajan kohtaan, Yleinen järjestelmänvalvoja voi kirja utua [teamsin hallinta portaaliin](https://admin.teams.microsoft.com/dashboard) ja **valita sitten** **Päivitä tila** -painikkeen Microsoft teamsin päivitys-kohdassa.</span><span class="sxs-lookup"><span data-stu-id="410fe-106">If you received communication about a Microsoft-driven automated upgrade from Skype for Business to Microsoft Teams, and you wish to postpone the automated upgrade to a later date, your Global Admin can log in to the [Teams Admin portal](https://admin.teams.microsoft.com/dashboard) and, after selecting the **Refresh Status** button under Microsoft Teams Upgrade, select the **Postpone** button.</span></span> <span data-ttu-id="410fe-107">Jos haluat nähdä uuden päivä määrän, jolloin vuokra ajan automaattinen päivitys Microsoft Teamsiin päivitetään, Päivitä teamsin hallinta portaalin sivu.</span><span class="sxs-lookup"><span data-stu-id="410fe-107">To see the new date for your tenant's automated upgrade to Microsoft Teams, refresh the Teams Admin portal page.</span></span>

<span data-ttu-id="410fe-108">**Huomautus:** **Postpone** -painike on käytettävissä vain, jos olet saanut viesti keskuksen ilmoituksen automaattisesta päivityksestä.</span><span class="sxs-lookup"><span data-stu-id="410fe-108">**Note:** The **Postpone** button will only be available if you have received the message center notification regarding the automated upgrade.</span></span> 

<span data-ttu-id="410fe-109">Yleisten järjestelmänvalvojien on myös suoritettava [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) , jotta saat lisä tietoja nykyisestä päivitys tilasta.</span><span class="sxs-lookup"><span data-stu-id="410fe-109">Global Admins can also run [Get-CsTeamsUpgradeStatus](https://docs.microsoft.com/powershell/module/skype/get-csteamsupgradestatus?view=skype-ps) to learn more about their current upgrade status.</span></span>
