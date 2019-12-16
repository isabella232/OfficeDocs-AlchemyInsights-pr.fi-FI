---
title: Työn kulun sähkö postia ei lähetetä
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 76b64323c9d34d49e9c6bd77c2cc7eff6d7c5402
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049370"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="0461b-102">Työn kulun sähkö postia ei lähetetä SharePoint-luetteloon tai-kirjastoon</span><span class="sxs-lookup"><span data-stu-id="0461b-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="0461b-103">Työn kulkujen sähkö postia ei lähetetä kaikille käyttäjille tai vain tietyille käyttäjille, tai näkyviin tulee virhe, **jonka mukaan Sähkö posti viestiä ei voi lähettää. Varmista, että sähkö posti viestissä on kelvollinen vastaanottaja**.</span><span class="sxs-lookup"><span data-stu-id="0461b-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="0461b-104">Tarkista, onko käyttäjä olemassa kyseisen sivustokokoelman **Kaikki henkilöt** -käyttö oikeudet-ryhmässä (käyttäjä tiedot-luettelossa).</span><span class="sxs-lookup"><span data-stu-id="0461b-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="0461b-105">Näyte suora URL-osoite<tenant>: https://<sitename>. SharePoint.com/sites//_layouts/15/People.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="0461b-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="0461b-106">Jos käyttäjää ei ole, varmista, että käyttäjä on kirjautuneena sivulle.</span><span class="sxs-lookup"><span data-stu-id="0461b-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="0461b-107">Jos kyseessä on ulkoinen käyttäjä, varmista, että heidän kutsunsa on hyväksytty.</span><span class="sxs-lookup"><span data-stu-id="0461b-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="0461b-108">Jos käyttäjä on olemassa käyttö oikeudet-ryhmässä, varmista, että sähkö posti osoite on oikein.</span><span class="sxs-lookup"><span data-stu-id="0461b-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="0461b-109">Jos käyttäjien Sähkö posti osoitetta ei ole määritetty tässä, luo kyseiselle käyttäjälle näyte hälytys, joka pakottaa kyseisen käyttäjä tilin synkronoinnin SharePoint-käyttäjä profiileista tähän sivustokokoelmaan.</span><span class="sxs-lookup"><span data-stu-id="0461b-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="0461b-110">Työn kuluista lähetetyt Sähkö posti viestit lähetetään sivustokokoelman järjestelmänvalvojille, mutta ei muille käyttäjille, ja http-protokollaa ei ole **kielletty <span>https:/URL/</span>_vti_bin/Client.xvc.SP.Utilities.Utility.sendemail**.</span><span class="sxs-lookup"><span data-stu-id="0461b-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="0461b-111">Katso [käyttö estetty, kun lähetät sähkö postia SharePoint-ryhmälle](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="0461b-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="0461b-112">Varmista myös, että **rajoitetun käytön käyttö oikeuden lukitus tilan** sivustokokoelman ominaisuus ei ole aktiivinen.</span><span class="sxs-lookup"><span data-stu-id="0461b-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="0461b-113">Aiheeseen liittyvät artikkelit</span><span class="sxs-lookup"><span data-stu-id="0461b-113">Related topics</span></span>
<span data-ttu-id="0461b-114">Haluatko kokeilla Microsoft Flow'ta SharePoint Onlinessa?</span><span class="sxs-lookup"><span data-stu-id="0461b-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="0461b-115">Luo työn kulku</span><span class="sxs-lookup"><span data-stu-id="0461b-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="0461b-116">SharePoint ja Flow</span><span class="sxs-lookup"><span data-stu-id="0461b-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


