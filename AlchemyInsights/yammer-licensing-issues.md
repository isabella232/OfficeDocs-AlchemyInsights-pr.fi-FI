---
title: Yammer-käyttö oikeus ongelmat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657273"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="a8878-102">Yammer-käyttö oikeus ongelmat</span><span class="sxs-lookup"><span data-stu-id="a8878-102">Yammer licensing issues</span></span>

<span data-ttu-id="a8878-103">Kaikilla käyttäjillä on oltava käyttö oikeus Yammer Enterprise-palvelun käyttöön, mutta oletusarvoisesti Yammer ei edellytä, että käyttäjillä on oikeus käyttää palvelua.</span><span class="sxs-lookup"><span data-stu-id="a8878-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="a8878-104">Kun järjestelmänvalvoja muuttaa asetusta niin, että se estää Microsoft 365-käyttäjät, joilla ei ole Yammer-käyttö oikeuksia, Yammer Enterprise-käyttö oikeutta ei voi käyttää.</span><span class="sxs-lookup"><span data-stu-id="a8878-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="a8878-105">Lisä tietoja on Ohje aiheessa [Yammer-käyttö oikeuksien hallinta Office 365-](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) sovelluksessa</span><span class="sxs-lookup"><span data-stu-id="a8878-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="a8878-106">Kun käyttö oikeuksia poistetaan käyttäjiltä, Yammer-ruutu ei ole enää näkyvissä ja muut palvelut voivat piilottaa ominaisuuksia käyttö oikeuksien poistamisen avulla.</span><span class="sxs-lookup"><span data-stu-id="a8878-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="a8878-107">Muissa tapa uksissa ominaisuudet voivat edelleen näkyä, mutta ne edellyttävät, että käyttö oikeus määritystä käytetään.</span><span class="sxs-lookup"><span data-stu-id="a8878-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="a8878-108">**Käyttäjä ei saa päivitettyä käyttö oikeutta**</span><span class="sxs-lookup"><span data-stu-id="a8878-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="a8878-109">Toisinaan käyttäjälle määritetään käyttö oikeus, mutta se ei edelleenkään pysty käyttämään Yammeria.</span><span class="sxs-lookup"><span data-stu-id="a8878-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="a8878-110">Viiveet tapahtuvat todennäköisemmin, kun massa käyttö oikeuden määritys on käynnissä.</span><span class="sxs-lookup"><span data-stu-id="a8878-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="a8878-111">Yammer-käyttäjiä ei ehkä päivitetä samassa järjestyksessä kuin käyttö oikeuksia muutetaan Azure AD:ssä, koska järjestelmä suoritetaan asynkronisesti.</span><span class="sxs-lookup"><span data-stu-id="a8878-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="a8878-112">Odota 24 tuntia, ennen kuin avaat tuki tapauksen ja ilmoitat käyttö oikeuksien synkronoinnin ongelmista.</span><span class="sxs-lookup"><span data-stu-id="a8878-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="a8878-113">**Bulk todistus-määritys**</span><span class="sxs-lookup"><span data-stu-id="a8878-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="a8878-114">Käyttö oikeudet voidaan määrittää hallinta keskuksen tai PowerShell-komento sarjojen kautta.</span><span class="sxs-lookup"><span data-stu-id="a8878-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="a8878-115">Lisä tietoja on Ohje aiheissa [käyttö oikeuksien määrittäminen käyttäjille](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ja käyttö [oikeuksien määrittäminen käyttäjä tileille Office 365 PowerShellin avulla](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="a8878-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="a8878-116">Microsoft-tuki ei anna ohjeita komento sarjojen luomiseen, mutta ohjeet ovat käytettävissä Yammer-käyttö oikeuksien määritystä varten.</span><span class="sxs-lookup"><span data-stu-id="a8878-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="a8878-117">Lisä tietoja on Ohje aiheessa [Yammer-käyttö oikeuksien hallinta Windows PowerShellin avulla](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="a8878-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>