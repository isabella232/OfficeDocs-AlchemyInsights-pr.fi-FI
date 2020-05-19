---
title: Haluatko merkitä verkkotunnuksen tai sähköpostin lähettäjän turvallisesti?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281145"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="1a75b-102">Haluatko merkitä verkkotunnuksen tai sähköpostin lähettäjän turvallisesti?</span><span class="sxs-lookup"><span data-stu-id="1a75b-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="1a75b-103">**Turvallisten lähettäjien luetteloiden** käyttöä ei suositella, koska se avaa organisaatiosi roskapostille, phishille ja väärentämishyökkäyksille.</span><span class="sxs-lookup"><span data-stu-id="1a75b-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="1a75b-104">Jos liiketoimintavaatimus kuitenkin on olemassa, **suosittelemme, että** käytät tähän Mail **[Flow -sääntöjä.](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)**</span><span class="sxs-lookup"><span data-stu-id="1a75b-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="1a75b-105">Ohjeemme varmistaa lähettäjän todennuksen (tarkistaa, että toimialueen lähettämistä ei vallu).</span><span class="sxs-lookup"><span data-stu-id="1a75b-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="1a75b-106">**Huomautus:** Emme suosittele väärien positiivisten tarkistusten hallintaa turvallisten lähettäjien luetteloiden avulla, koska roskapostin suodattamiseen tehdyt poikkeukset voivat avata organisaatiosi suojaushyökkäyksille.</span><span class="sxs-lookup"><span data-stu-id="1a75b-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="1a75b-107">Jos käyttäjäsi saavat roskapostiksi tai roskapostiksi virheellisesti merkittyjä viestejä, **[ilmoita viesteistä ja tiedostoista Microsoftille.](https://protection.office.com/reportsubmission)**</span><span class="sxs-lookup"><span data-stu-id="1a75b-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="1a75b-108">Turvalliset lähettäjät Outlookissa, Sallittu lähettäjäluettelo tai sallittu toimialueluettelo roskapostin vastaisissa käytännöissä **tulisi välttää,** koska lähettäjät ohittavat kaiken roskapostin, väärentämisen ja phish-suojauksen sekä lähettäjän todennuksen (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="1a75b-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="1a75b-109">Tätä menetelmää käytetään parhaiten vain tilapäisissä testeissä.</span><span class="sxs-lookup"><span data-stu-id="1a75b-109">This method is best used for temporary testing only.</span></span>
