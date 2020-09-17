---
title: Haluatko merkitä toimi alueen tai sähkö postin lähettäjän turvalliseksi?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803242"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="2463b-102">Haluatko merkitä toimi alueen tai sähkö postin lähettäjän turvalliseksi?</span><span class="sxs-lookup"><span data-stu-id="2463b-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="2463b-103">**Turvallisten lähettäjien luetteloiden käyttöä ei suositella** , koska se avaa organisaation roska posti-, Phish-ja huijaus hyökkäyksille.</span><span class="sxs-lookup"><span data-stu-id="2463b-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="2463b-104">Jos liiketoiminta vaatimus on olemassa, **suosittelemme** , että käytät siihen **[sähkö postin kulku sääntöjä](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** .</span><span class="sxs-lookup"><span data-stu-id="2463b-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="2463b-105">Ohja uksen avulla varmistat, että lähettäjän todennus (tarkistaa, että lähettävä toimi alue ei ole väärennetty).</span><span class="sxs-lookup"><span data-stu-id="2463b-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="2463b-106">**Huomautus**: emme suosittele väärien positiivisten viestien hallintaa turvallisten lähettäjien luetteloiden avulla, koska roska posti suodatukseen liittyvät poikkeukset voivat avata organisaatiosi tieto turva hyökkäyksille.</span><span class="sxs-lookup"><span data-stu-id="2463b-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="2463b-107">Jos käyttäjä lähettää viestejä, jotka on merkitty virheellisesti roska postiksi tai roska postiksi, **[Ilmianna viestit ja tiedostot Microsoftille](https://protection.office.com/reportsubmission)**.</span><span class="sxs-lookup"><span data-stu-id="2463b-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="2463b-108">Turvalliset lähettäjät Outlookissa, sallittujen lähettäjien luettelossa tai sallittujen toimi alueiden luettelossa roska postin vastaisessa politiikassa **tulee välttää** , koska lähettäjät ohittavat kaikki roska posti-, huijaus-ja Phish-suoja uksen ja lähettäjän todennuksen (SPF, DKIM, dMarc).</span><span class="sxs-lookup"><span data-stu-id="2463b-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="2463b-109">Tätä menetelmää käytetään parhaiten vain väliaikaiseen testaukseen.</span><span class="sxs-lookup"><span data-stu-id="2463b-109">This method is best used for temporary testing only.</span></span>
