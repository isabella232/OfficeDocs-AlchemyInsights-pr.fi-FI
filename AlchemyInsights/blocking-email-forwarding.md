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
ms.openlocfilehash: 2f3528375d251542fd82761d00c776706de2e23c
ms.sourcegitcommit: f7b82f75a5400e992ecbd48a666783354e2e2871
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/15/2020
ms.locfileid: "48473098"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="6b3c6-102">Sähkö postin lähettämisen estäminen tai eston poistaminen</span><span class="sxs-lookup"><span data-stu-id="6b3c6-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="6b3c6-103">Jos haluat ottaa sähkö postin uudelleenohjauksen käyttöön tai poistaa sen käytöstä tietyssä posti laatikossa, katso [sähkö postin uudelleenohjauksen määrittäminen](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span><span class="sxs-lookup"><span data-stu-id="6b3c6-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="6b3c6-104">Vuokra ajan tasolla ulkoista lähetystä voidaan hallita lähtevällä roska posti käytännöllä.</span><span class="sxs-lookup"><span data-stu-id="6b3c6-104">On the tenant level, control of external forwarding is done using the outbound spam policy.</span></span> <span data-ttu-id="6b3c6-105">Voit tarkistaa lähtevän roska postin suodatus käytännöt tieto turva-ja yhteensopivuus keskuksesta [Here] ( https://protection.office.com/antispam) tai käyttämällä [Get-Hostedoutboundspamfilttpolicy-komentoa](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span><span class="sxs-lookup"><span data-stu-id="6b3c6-105">You can check the outbound spam filter policy from Security and Compliance Center [here] (https://protection.office.com/antispam) or by using the [Get-HostedOutboundSpamFilterPolicy command](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span></span>

<span data-ttu-id="6b3c6-106">Jos saat seuraavan virhe ilmoituksen: **"550 5.7.520 käyttö estetty, organisaatiosi ei salli ulkoista edelleenlähetystä"**, varmista, että käytännöt on määritetty niin, että ulkoinen automaattinen edelleensiirto on käytössä.</span><span class="sxs-lookup"><span data-stu-id="6b3c6-106">If you are getting the following error: **“550 5.7.520 Access denied, Your organization does not allow external forwarding”**, please make sure the policy is configured to enable External Auto-forward.</span></span>

<span data-ttu-id="6b3c6-107">**Huomautus:** On suositeltavaa, että ulkoinen automaattinen siirto ei ole käytössä oletusarvoisessa lähtevän postin roska posti suodatus käytännössä ja että se on käytettävissä vain niitä käyttäjiä varten, jotka tarvitsevat ulkoista edelleenlähetystä luomalla mukautetun käytäntöjen näille käyttäjille.</span><span class="sxs-lookup"><span data-stu-id="6b3c6-107">**Note:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="6b3c6-108">Lisä tietoja on artikkelissa [ulkoinen sähkö postin lähettäminen uudelleen Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)-sovelluksessa.</span><span class="sxs-lookup"><span data-stu-id="6b3c6-108">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>