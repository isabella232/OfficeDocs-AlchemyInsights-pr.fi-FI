---
title: Työnkulun sähköposti ei lähetetä
ms.author: efrene
author: efrene
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
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530867"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="3c51d-102">Työnkulun sähköposti lähetetään ei ole SharePoint-luettelossa tai kirjastossa</span><span class="sxs-lookup"><span data-stu-id="3c51d-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="3c51d-103">Kaikki käyttäjät tai vain tietyille käyttäjille ei lähetetä sähköposti-työnkulkuja tai nähdä virhe **sähköpostiviestiä ei voi lähettää. Varmista, että sähköpostiviestillä on kelvollinen vastaanottaja**.</span><span class="sxs-lookup"><span data-stu-id="3c51d-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="3c51d-104">Tarkista, onko käyttäjä ole **Kaikkien henkilöiden** oikeudet ryhmässä (käyttäjätietoluetteloon) kyseisen sivustokokoelman.</span><span class="sxs-lookup"><span data-stu-id="3c51d-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="3c51d-105">Näyte suoraan URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx? MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="3c51d-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="3c51d-106">Jos käyttäjä ei ole, varmista, että käyttäjä on kirjautunut sivulle.</span><span class="sxs-lookup"><span data-stu-id="3c51d-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="3c51d-107">Jos kyseessä on ulkoinen käyttäjä, varmista, että niiden kutsu on hyväksytty.</span><span class="sxs-lookup"><span data-stu-id="3c51d-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="3c51d-108">Jos käyttäjä ole ryhmän käyttöoikeudet, varmista, että sähköpostiosoite on oikein.</span><span class="sxs-lookup"><span data-stu-id="3c51d-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="3c51d-109">Jos käyttäjät sähköpostiosoitetta ei ole määritetty tässä, Luo malli-ilmoitus, joka pakottaa käyttäjätilin synkronointi käyttäjän profiilit SharePoint-sivustokokoelman käyttäjälle.</span><span class="sxs-lookup"><span data-stu-id="3c51d-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="3c51d-110">Työnkulut-sähköposti lähetetään sivustokokoelman järjestelmänvalvojat, mutta ei muiden käyttäjien ja tulla seuraava virhe **kiellettyä HTTP <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span><span class="sxs-lookup"><span data-stu-id="3c51d-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="3c51d-111">On [Estetty, kun lähetät sähköpostia SharePoint-ryhmään](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span><span class="sxs-lookup"><span data-stu-id="3c51d-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="3c51d-112">Tarkista myös sivustokokoelman ominaisuuden **käyttöoikeus on rajoitettu käyttöoikeus lockdown tilassa** ei ole aktiivinen.</span><span class="sxs-lookup"><span data-stu-id="3c51d-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="3c51d-113">Aiheeseen liittyvät artikkelit</span><span class="sxs-lookup"><span data-stu-id="3c51d-113">Related topics</span></span>
<span data-ttu-id="3c51d-114">Jos haluat kokeilla Microsoft SharePoint Online-Flow?</span><span class="sxs-lookup"><span data-stu-id="3c51d-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="3c51d-115">Luo työnkulku</span><span class="sxs-lookup"><span data-stu-id="3c51d-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="3c51d-116">SharePoint- ja</span><span class="sxs-lookup"><span data-stu-id="3c51d-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


