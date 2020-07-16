---
title: Yammerin käyttöoikeusongelmat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148238"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="ea04a-102">Yammerin käyttöoikeusongelmat</span><span class="sxs-lookup"><span data-stu-id="ea04a-102">Yammer licensing issues</span></span>

<span data-ttu-id="ea04a-103">Kaikilla käyttäjillä on oltava yammer-yrityspalvelun käyttöoikeus, mutta oletusarvoisesti Yammer ei edellytä, että käyttäjillä on palvelun käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="ea04a-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="ea04a-104">Kun järjestelmänvalvoja muuttaa asetusta estääkseen Microsoft 365 -käyttäjät, joilla ei ole Yammer-käyttöoikeuksia, käyttäjät, joille ei ole määritetty Yammer Enterprise -käyttöoikeutta, eivät voi käyttää Yammer-palvelua.</span><span class="sxs-lookup"><span data-stu-id="ea04a-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="ea04a-105">Lisätietoja on [ohjeaiheessa Yammer-käyttöoikeuksien hallinta Office 365:ssä](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="ea04a-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="ea04a-106">Kun käyttöoikeudet poistetaan käyttäjiltä, Yammer-ruutua ei enää näytetä, ja muut palvelut voivat piilottaa ominaisuuksia käyttöoikeuksien poistamisen avulla.</span><span class="sxs-lookup"><span data-stu-id="ea04a-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="ea04a-107">Muissa tapauksissa ominaisuudet voivat silti näkyä, mutta ne edellyttävät käyttöoikeuden myöntämistä.</span><span class="sxs-lookup"><span data-stu-id="ea04a-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="ea04a-108">**Käyttäjän lisenssiä ei päivitetä**</span><span class="sxs-lookup"><span data-stu-id="ea04a-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="ea04a-109">Joskus käyttäjälle on määritetty käyttöoikeus, mutta hän ei edelleenkään pysty käyttämään Yammeria.</span><span class="sxs-lookup"><span data-stu-id="ea04a-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="ea04a-110">Viiveet ovat todennäköisempiä, kun joukkokäyttöoikeuden määritys on käynnissä.</span><span class="sxs-lookup"><span data-stu-id="ea04a-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="ea04a-111">Yammerin käyttäjiä ei ehkä päivitetä samassa järjestyksessä kuin käyttöoikeuksia muutetaan Azure AD:ssä, koska järjestelmä toimii asynkronisesti.</span><span class="sxs-lookup"><span data-stu-id="ea04a-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="ea04a-112">Odota enintään 24 tuntia ennen tukitapauksen avaamista ja ilmoita käyttöoikeuksien synkronointiongelmista.</span><span class="sxs-lookup"><span data-stu-id="ea04a-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="ea04a-113">**Joukkolisenssin määritys**</span><span class="sxs-lookup"><span data-stu-id="ea04a-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="ea04a-114">Käyttöoikeudet voidaan määrittää hallintakeskuksen tai PowerShell-komentosarjojen kautta.</span><span class="sxs-lookup"><span data-stu-id="ea04a-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="ea04a-115">Lisätietoja on ohjeissa [Käyttöoikeuksien määrittäminen käyttäjille](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ja [Käyttöoikeuksien määrittäminen käyttäjätileille Office 365 PowerShellin avulla](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="ea04a-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="ea04a-116">Microsoft-tuki ei tue komentosarjojen luomista, mutta Yammer-käyttöoikeusmäärityksen ohjeet ovat käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="ea04a-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="ea04a-117">Lisätietoja on [ohjeaiheessa Yammer-käyttöoikeuksien hallinta Windows PowerShellin avulla](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="ea04a-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>