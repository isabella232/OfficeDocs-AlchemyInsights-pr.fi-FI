---
title: Työnkulun sähköpostia ei lähetetä
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 391d3a2dcc2676a405065115f375c802d2492119
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766130"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="67ec0-102">Työnkulun sähköpostia ei lähetetä SharePoint-luetteloon tai kirjastoon</span><span class="sxs-lookup"><span data-stu-id="67ec0-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="67ec0-103">Työnkulkujen sähköpostia ei lähetetä kaikille käyttäjille tai vain tietyille käyttäjille, tai näet virheen **Sähköpostiviestiä ei voi lähettää. Varmista, että sähköpostiviestissä on kelvollinen vastaanottaja**.</span><span class="sxs-lookup"><span data-stu-id="67ec0-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="67ec0-104">Tarkista, onko käyttäjä kyseisen sivustokokoelman **Kaikki henkilöt -käyttöoikeusryhmässä** (käyttäjätietoluettelo).</span><span class="sxs-lookup"><span data-stu-id="67ec0-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="67ec0-105">Esimerkki suorasta<tenant>URL-osoitteesta: https:// .sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId=0 (jäsenyysryhmä)=0</span><span class="sxs-lookup"><span data-stu-id="67ec0-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="67ec0-106">Jos käyttäjää ei ole, varmista, että käyttäjä on kirjautunut sivulle.</span><span class="sxs-lookup"><span data-stu-id="67ec0-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="67ec0-107">Jos se on ulkoinen käyttäjä, varmista, että kutsu on hyväksytty.</span><span class="sxs-lookup"><span data-stu-id="67ec0-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="67ec0-108">Jos käyttäjä on käyttöoikeusryhmässä, varmista, että sähköpostiosoite on oikein.</span><span class="sxs-lookup"><span data-stu-id="67ec0-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="67ec0-109">Jos käyttäjien sähköpostiosoitetta ei ole määritetty tässä, luo kyseiselle käyttäjälle esimerkkiilmoitus, joka pakottaa kyseisen käyttäjätilin synkronoinnin SharePointin käyttäjäprofiileista tähän sivustokokoelmaan.</span><span class="sxs-lookup"><span data-stu-id="67ec0-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="67ec0-110">Työnkulkujen sähköposti lähetetään sivustokokoelman järjestelmänvalvojille, mutta ei muille käyttäjille, ja virhe **HTTP Kielletty <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="67ec0-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="67ec0-111">Lisätietoja [on ohjeaiheessa Käyttö estetty, kun lähetät sähköpostia SharePoint-ryhmään](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="67ec0-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="67ec0-112">Varmista myös, että **rajoitetun käytön käyttäjän käyttöoikeuksien lukitustilan** sivustokokoelmaominaisuus ei ole aktiivinen.</span><span class="sxs-lookup"><span data-stu-id="67ec0-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="67ec0-113">Aiheeseen liittyvät artikkelit</span><span class="sxs-lookup"><span data-stu-id="67ec0-113">Related topics</span></span>
<span data-ttu-id="67ec0-114">Haluatko kokeilla Microsoft Flow'ta SharePoint Onlinessa?</span><span class="sxs-lookup"><span data-stu-id="67ec0-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="67ec0-115">Luo työnkulku</span><span class="sxs-lookup"><span data-stu-id="67ec0-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="67ec0-116">SharePoint ja Flow</span><span class="sxs-lookup"><span data-stu-id="67ec0-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


