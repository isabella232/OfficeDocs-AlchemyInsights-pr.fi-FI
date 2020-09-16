---
title: Työn kulun Sähkö posti viestiä ei lähetetä
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748986"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="edef0-102">Työn kulun Sähkö posti viestiä ei lähetetä SharePoint-luettelolle tai-kirjastolle</span><span class="sxs-lookup"><span data-stu-id="edef0-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="edef0-103">Työn kulkujen Sähkö posti viestejä ei lähetetä kaikille käyttäjille tai vain tietyille käyttäjille, tai näet virhe ilmoituksen, **jonka mukaan Sähkö posti viestiä ei voi lähettää. Varmista, että sähkö posti viestissä on kelvollinen vastaanottaja**.</span><span class="sxs-lookup"><span data-stu-id="edef0-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="edef0-104">Tarkista, onko käyttäjä olemassa kyseisen sivustokokoelman **Kaikki henkilöt** -käyttö oikeudet-ryhmässä (käyttäjä tiedot-luettelossa).</span><span class="sxs-lookup"><span data-stu-id="edef0-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="edef0-105">Esimerkki suora URL-osoitteesta: https:// <tenant> . SharePoint.com/sites/ <sitename> /_layouts/15/People.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="edef0-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="edef0-106">Jos käyttäjää ei ole olemassa, varmista, että käyttäjä on kirjautunut sivulle.</span><span class="sxs-lookup"><span data-stu-id="edef0-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="edef0-107">Jos kyseessä on ulkoinen käyttäjä, varmista, että hänen kutsunsa on hyväksytty.</span><span class="sxs-lookup"><span data-stu-id="edef0-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="edef0-108">Jos käyttäjä on olemassa käyttö oikeudet-ryhmässä, varmista, että sähkö posti osoite on oikein.</span><span class="sxs-lookup"><span data-stu-id="edef0-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="edef0-109">Jos käyttäjien Sähkö posti osoitetta ei ole annettu tässä, luo kyseiselle käyttäjälle esimerkki ilmoitus, joka pakottaa kyseisen käyttäjä tilin synkronoinnin SharePointin käyttäjä profiileista tähän sivustokokoelmaan.</span><span class="sxs-lookup"><span data-stu-id="edef0-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="edef0-110">Työn kulkujen Sähkö posti viestit lähetetään sivustokokoelman järjestelmänvalvojille, mutta ei muille käyttäjille, ja Katso http-virhe \*\* <span>https:</span>//_vti_bin/Client.xvc.SP.Utilities.Utility.sendemail\*\*.</span><span class="sxs-lookup"><span data-stu-id="edef0-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="edef0-111">Katso [käyttö estetty, kun lähetät sähkö postia SharePoint-ryhmälle](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="edef0-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="edef0-112">Varmista myös, että **rajoitetun käytön käyttö oikeuksien lukitus tilan** sivustokokoelman ominaisuus ei ole aktiivinen.</span><span class="sxs-lookup"><span data-stu-id="edef0-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="edef0-113">Aiheeseen liittyvät artikkelit</span><span class="sxs-lookup"><span data-stu-id="edef0-113">Related topics</span></span>
<span data-ttu-id="edef0-114">Haluatko kokeilla Microsoft Flow'ta SharePoint Onlinessa?</span><span class="sxs-lookup"><span data-stu-id="edef0-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="edef0-115">Työn kulun luominen</span><span class="sxs-lookup"><span data-stu-id="edef0-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="edef0-116">SharePoint ja Flow</span><span class="sxs-lookup"><span data-stu-id="edef0-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


