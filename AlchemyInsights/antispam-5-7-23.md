---
title: Roskapostin esto - 5.7.23
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
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676494"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="d8163-102">Korjaa sähköpostin toimitusongelmat virhekoodille 5.7.23</span><span class="sxs-lookup"><span data-stu-id="d8163-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="d8163-103">Tarkista toimialueesi SPF-DNS-tietue verkossa julkisesti saatavilla olevassa SPF- tai DNS-tietueen tarkistuksessa.</span><span class="sxs-lookup"><span data-stu-id="d8163-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="d8163-104">Varmista, että Microsoft ei tunnistanut lähtevää viestiä roskapostiksi ja että se reititetään [suuren riskin toimituspoolin](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages)kautta.</span><span class="sxs-lookup"><span data-stu-id="d8163-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="d8163-105">Suuren riskin toimituspoolissa olevat viestit eivät läpäise SPF-tarkistuksia, joten kohdesähköpostiorganisaatio ei hyväksy niitä.</span><span class="sxs-lookup"><span data-stu-id="d8163-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="d8163-106">Jos ongelma ei poistu, sinun on ehkä otettava yhteyttä sen sähköpostiisännän järjestelmänvalvojaan, johon yrität lähettää sähköpostia.</span><span class="sxs-lookup"><span data-stu-id="d8163-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="d8163-107">Merkitse muistisanomassa käytettävissä oleva yksityiskohtainen ulkoinen virhe muistiin.</span><span class="sxs-lookup"><span data-stu-id="d8163-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="d8163-108">Microsoftin tuki ei ehkä voi auttaa enempää.</span><span class="sxs-lookup"><span data-stu-id="d8163-108">Microsoft support may not be able to assist further.</span></span>
