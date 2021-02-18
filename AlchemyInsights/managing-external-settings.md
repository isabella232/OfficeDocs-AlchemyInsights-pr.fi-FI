---
title: Ulkoisten asetusten hallinta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294212"
---
# <a name="managing-external-settings"></a><span data-ttu-id="a27d5-102">Ulkoisten asetusten hallinta</span><span class="sxs-lookup"><span data-stu-id="a27d5-102">Managing External Settings</span></span>

<span data-ttu-id="a27d5-103">**Ilmoitus**</span><span class="sxs-lookup"><span data-stu-id="a27d5-103">**Announcement**</span></span>

- <span data-ttu-id="a27d5-104">[WebView-kirjautumistuen peruuttaminen Googlesta 4. tammikuuta 2021 alkaen.](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support)</span><span class="sxs-lookup"><span data-stu-id="a27d5-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="a27d5-105">Testaa, vaikuttaako sovellustesi yhteensopivuus Googlen ohjeiden mukaisesti</span><span class="sxs-lookup"><span data-stu-id="a27d5-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="a27d5-106">Varmista, että käytät järjestelmän verkkonäkymää tai järjestelmäselainta, kun kirjaudut sisään käyttäjiisi kuluttaja-Google-tileillä</span><span class="sxs-lookup"><span data-stu-id="a27d5-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="a27d5-107">**Kutsuasetusten hallinta**</span><span class="sxs-lookup"><span data-stu-id="a27d5-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="a27d5-108">Varmista, että olet [määrittänyt ulkoisen yhteistyön asetukset](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) niin, että asianmukaiset henkilöt voivat lähettää kutsuja.</span><span class="sxs-lookup"><span data-stu-id="a27d5-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="a27d5-109">**Vieraskäyttöoikeuksien hallinta**</span><span class="sxs-lookup"><span data-stu-id="a27d5-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="a27d5-110">Yleiset järjestelmänvalvojat voivat hallita hakemiston vieraskäyttöoikeuksia Azure-portaalin kautta määrittämällä vieraskäyttöoikeudet Ulkoisen yhteistyön asetukset -sivulla.</span><span class="sxs-lookup"><span data-stu-id="a27d5-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="a27d5-111">[Lue lisää tästä asetusasetuksesta.](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="a27d5-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="a27d5-112">Jos haluat vieraiden voivan käyttää sovelluksia, kuten Teams tai SharePoint, varmista, että olet määrittänyt sovellukset sallimaan vieraskäyttö.</span><span class="sxs-lookup"><span data-stu-id="a27d5-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="a27d5-113">Lisätietoja Teamsin [asetuksista ja](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) [SharePointista.](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="a27d5-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="a27d5-114">**Kutsujen määrittäminen:**</span><span class="sxs-lookup"><span data-stu-id="a27d5-114">**Configuring invitations:**</span></span>

- [<span data-ttu-id="a27d5-115">Ota B2B:n ulkoinen yhteistyö käyttöön ja hallitse sitä, ketkä voivat kutsua vieraita</span><span class="sxs-lookup"><span data-stu-id="a27d5-115">Enable B2B external collaboration and manage who can invite guests</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="a27d5-116">Tiettyjen organisaatioiden käyttäjien kutsujen salliminen tai estäminen</span><span class="sxs-lookup"><span data-stu-id="a27d5-116">Allow or block invitations to users from specific organizations</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="a27d5-117">**Sallittujen tunnistetietojen palveluntarjoajien määrittäminen:**</span><span class="sxs-lookup"><span data-stu-id="a27d5-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="a27d5-118">Google Federation</span><span class="sxs-lookup"><span data-stu-id="a27d5-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="a27d5-119">Suora liittouminen</span><span class="sxs-lookup"><span data-stu-id="a27d5-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="a27d5-120">Kertatunnistus sähköpostitse</span><span class="sxs-lookup"><span data-stu-id="a27d5-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
