---
title: 726 sähkö postin siirron estäminen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219852"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="df1f2-102">Sähkö postin lähettämisen estäminen tai eston poistaminen</span><span class="sxs-lookup"><span data-stu-id="df1f2-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="df1f2-103">Jos haluat ottaa sähkö postin uudelleenohjauksen käyttöön tai poistaa sen käytöstä tietyssä posti laatikossa, katso [sähkö postin uudelleenohjauksen määrittäminen](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="df1f2-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="df1f2-104">Vuokra ajan tasolla ulkoista lähetystä voidaan hallita lähtevän roska postin vastaista käytäntöä käyttäen.</span><span class="sxs-lookup"><span data-stu-id="df1f2-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="df1f2-105">Jos se on poistettu käytöstä tai se on automaattinen, se voi estää sähkö postin lähettämisen "550 5.7.520 käyttö estetty-virheen vuoksi, joten organisaatiosi ei salli ulkoista lähetystä"-virhe.</span><span class="sxs-lookup"><span data-stu-id="df1f2-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="df1f2-106">Tämän jälkeen, jos siirto on tarkoitus estää, se on virhe, jonka käyttäjät näkevät.</span><span class="sxs-lookup"><span data-stu-id="df1f2-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="df1f2-107">Jos edelleenlähetystä ei estetä, varmista, että käytännöt on määritetty niin, että ulkoinen Autoforward on käytössä.</span><span class="sxs-lookup"><span data-stu-id="df1f2-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="df1f2-108">Voit tarkistaa lähtevän roska postin suodatus käytännöt tieto turva-ja yhteensopivuus keskuksesta tai suorittamalla komennon Get-Hostedoutboundspamfilttpolicy | FL Name, Autofordingingmode.</span><span class="sxs-lookup"><span data-stu-id="df1f2-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="df1f2-109">Jos haluat määrittää automaattisen edelleenkäytön eston, sama komento kertoo nyt käytännössä.</span><span class="sxs-lookup"><span data-stu-id="df1f2-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="df1f2-110">Huomautus: on suositeltavaa, että ulkoinen automaattinen edelleenlähetys on poistettu käytöstä lähtevien roska posti suodattimen oletus käytännöllä ja että se on käytettävissä vain niitä käyttäjiä varten, jotka tarvitsevat ulkoista edelleenlähetystä luomalla mukautetun käytäntöjen näille käyttäjille.</span><span class="sxs-lookup"><span data-stu-id="df1f2-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="df1f2-111">Lisä tietoja on artikkelissa [ulkoinen sähkö postin lähettäminen uudelleen Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)-sovelluksessa.</span><span class="sxs-lookup"><span data-stu-id="df1f2-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>