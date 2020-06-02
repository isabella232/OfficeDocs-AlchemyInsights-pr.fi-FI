---
title: Roskapostin torjunta - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 8122b409a731a5fcc46c718aff1eeda07e26890b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506440"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="58063-102">Virhekoodin 5.7.23 sähköpostin toimitusongelmien korjaaminen</span><span class="sxs-lookup"><span data-stu-id="58063-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="58063-103">Tarkista toimialueesi SPF DNS -tietue julkisesti saatavilla olevasta SPF- tai DNS-tietueiden tarkistamisesta verkossa.</span><span class="sxs-lookup"><span data-stu-id="58063-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="58063-104">Varmista, että Microsoft ei tunnistanut lähtevää viestiä roskapostiksi ja että se reititetään [suuren riskin toimitusvarannon](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)kautta.</span><span class="sxs-lookup"><span data-stu-id="58063-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="58063-105">Suuren riskin toimitusvarannon viestit eivät läpäise SPF-tarkistuksia, joten kohdesähköpostiorganisaatio ei hyväksy niitä.</span><span class="sxs-lookup"><span data-stu-id="58063-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="58063-106">Jos ongelma ei poistu, sinun on ehkä otettava yhteyttä sen sähköpostiisännän järjestelmänvalvojaan, johon yrität lähettää sähköpostia.</span><span class="sxs-lookup"><span data-stu-id="58063-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="58063-107">Merkitse muistiin poistumisviestissä käytettävissä oleva yksityiskohtainen ulkoinen virhe.</span><span class="sxs-lookup"><span data-stu-id="58063-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="58063-108">Microsoftin tuki ei ehkä voi auttaa enempää.</span><span class="sxs-lookup"><span data-stu-id="58063-108">Microsoft support may not be able to assist further.</span></span>
