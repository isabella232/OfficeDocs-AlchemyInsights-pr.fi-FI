---
title: Roskaposti - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821408"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="fa2d2-102">Sähköpostin toimitusongelman korjaus virhekoodille 5.7.23</span><span class="sxs-lookup"><span data-stu-id="fa2d2-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="fa2d2-103">Tarkista toimialueen SPF DNS -tietue internetissä yleisesti saatavilla olevan SPF- tai DNS-tietueiden tarkistuspalvelun kautta.</span><span class="sxs-lookup"><span data-stu-id="fa2d2-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="fa2d2-104">Varmista, että Microsoft ei ole tunnistanut lähtevää viestiä roskapostiksi ja että se reititettiin Suuren riskin [toimitus poolin kautta.](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="fa2d2-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="fa2d2-105">Suuren riskin toimitus poolin viestit eivät läpäise SPF-tarkistuksia, joten kohdesähköpostiorganisaatio ei hyväksy niitä.</span><span class="sxs-lookup"><span data-stu-id="fa2d2-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="fa2d2-106">Jos ongelma jatkuu, sinun on ehkä otettava yhteyttä sen sähköpostipalvelimen järjestelmänvalvojaan, jolle yrität lähettää sähköpostia.</span><span class="sxs-lookup"><span data-stu-id="fa2d2-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="fa2d2-107">Merkitse yksityiskohtainen ulkoinen virhe muistiin ilmoituksen ilmoitusviestin ilmoituksista.</span><span class="sxs-lookup"><span data-stu-id="fa2d2-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="fa2d2-108">Microsoft-tuki ei ehkä voi auttaa enempää.</span><span class="sxs-lookup"><span data-stu-id="fa2d2-108">Microsoft support may not be able to assist further.</span></span>
