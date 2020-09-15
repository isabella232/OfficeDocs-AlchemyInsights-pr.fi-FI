---
title: Roska postin esto-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717322"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="81038-102">Sähkö postin välitys ongelmien korjaaminen virhe koodissa 5.7.23</span><span class="sxs-lookup"><span data-stu-id="81038-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="81038-103">Varmista, että toimi alueesi SPF DNS-tietue on julkisesti saatavilla olevassa SPF-tai DNS-tietueiden tarkistuksessa verkossa.</span><span class="sxs-lookup"><span data-stu-id="81038-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="81038-104">Varmista, että Microsoft ei ole määrittänyt lähtevää viestiä roska postiksi, ja reititetty [suuren riskin lähetys varannon](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)kautta.</span><span class="sxs-lookup"><span data-stu-id="81038-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="81038-105">Suuren riskin vastaanotto varannon viestit eivät läpäise SPF-tarkistuksia, joten kohde Sähkö posti organisaatio ei hyväksy niitä.</span><span class="sxs-lookup"><span data-stu-id="81038-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="81038-106">Jos ongelma jatkuu, sinun on ehkä otettava yhteyttä sen Sähkö posti palvelimen järjestelmänvalvojaan, johon yrität lähettää sähkö postia.</span><span class="sxs-lookup"><span data-stu-id="81038-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="81038-107">Merkitse muistiin palautus viestissä oleva tarkka ulkoinen virhe.</span><span class="sxs-lookup"><span data-stu-id="81038-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="81038-108">Microsoft-tuki ei ehkä pysty auttamaan.</span><span class="sxs-lookup"><span data-stu-id="81038-108">Microsoft support may not be able to assist further.</span></span>
