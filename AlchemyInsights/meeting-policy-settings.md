---
title: Kokouskäytäntöasetukset
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
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704603"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="59a4b-102">Kokouskäytäntöjen hallinta Microsoft Teamsissa</span><span class="sxs-lookup"><span data-stu-id="59a4b-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="59a4b-103">**Huomautus: käytäntömuutokset tulevat voimaan käyttäjille jopa 24 tunnin kuluessa.**</span><span class="sxs-lookup"><span data-stu-id="59a4b-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="59a4b-104">Et ehkä voi tehdä muutoksia juuri luotuihin käytäntöihin välittömästi. odota 4 tuntia ja yritä muokata juuri luotua käytäntöä uudelleen.</span><span class="sxs-lookup"><span data-stu-id="59a4b-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="59a4b-105">Kokouskäytäntöjen avulla hallitaan ominaisuuksia, jotka kokouksen osallistujat voivat käyttää kokouksissa, jotka organisaation käyttäjät ajoittaa.</span><span class="sxs-lookup"><span data-stu-id="59a4b-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="59a4b-106">Joitakin kokouskäytäntöjen ominaisuuksia ei ehkä vielä ole otettu käyttöön Teams-hallintakeskuksessa (ohjeissa on merkintä "tulossa pian").</span><span class="sxs-lookup"><span data-stu-id="59a4b-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="59a4b-107">Tässä tapauksessa tai jos saat Microsoft Teams -hallintakeskuksessa virheilmoituksen "Käytäntöä ei voi päivittää juuri nyt, mutta yritä myöhemmin uudelleen", suosittelemme, että luot tai muokkaat Teamsin kokouskäytäntöjä PowerShellin avulla.</span><span class="sxs-lookup"><span data-stu-id="59a4b-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="59a4b-108">Lisätietoja kokouskäytännöistä on seuraavissa resursseissa:</span><span class="sxs-lookup"><span data-stu-id="59a4b-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="59a4b-109">Lisätietoja käytännön luomisesta, muutosten luomisesta ja käyttäjien määrittämisestä käytäntöön on teamsin [kokouskäytäntöjen hallinta -kohdassa.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="59a4b-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="59a4b-110">Jos haluat tehdä käytäntömuutoksia PowerShellin cmdlet-komentojen avulla, tutustu [Teams PowerShellin yleiskatsaukseen.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="59a4b-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="59a4b-111">Sinun on käytettävä [Teamsin kokouskäytäntöjen Skype for Business PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) -moduulia.</span><span class="sxs-lookup"><span data-stu-id="59a4b-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="59a4b-112">Saat [lisätietoja \*-CsTeamsMeetingPolicy-cmdlet-komentojen](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) ohjeista.</span><span class="sxs-lookup"><span data-stu-id="59a4b-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

