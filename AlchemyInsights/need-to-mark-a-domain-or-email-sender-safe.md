---
title: Tarvitseeko sinun merkitä toimialue tai sähköpostin lähettäjä turvalliseksi?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792129"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="7ccd3-102">Tarvitseeko sinun merkitä toimialue tai sähköpostin lähettäjä turvalliseksi?</span><span class="sxs-lookup"><span data-stu-id="7ccd3-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="7ccd3-103">Turvallisten **lähettäjien luetteloiden käyttöä** ei suositella, koska se avaa organisaatiosi roskaposti-, osoite- ja osoitetushyökkäyksille.</span><span class="sxs-lookup"><span data-stu-id="7ccd3-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="7ccd3-104">Jos liiketoimintaa kuitenkin vaaditaan, suosittelemme käyttämään **tähän** **[postinkulkusääntöjä.](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)**</span><span class="sxs-lookup"><span data-stu-id="7ccd3-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="7ccd3-105">Ohjeemme varmistavat lähettäjän todennuksen (varmistaa, että toimialueen lähetystä ei osoiteta).</span><span class="sxs-lookup"><span data-stu-id="7ccd3-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="7ccd3-106">**Huomautus:** Emme suosittele virheellisten positiivisten tietojen hallintaa turvallisten lähettäjien luetteloiden avulla, koska roskapostisuodatuksen poikkeukset voivat avata organisaatiosi suojaushyökkäyksiin.</span><span class="sxs-lookup"><span data-stu-id="7ccd3-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="7ccd3-107">Jos käyttäjäsi saavat virheellisesti roskapostiksi merkittyjä viestejä, ilmoita viesteistä ja tiedostoista **[Microsoftille.](https://protection.office.com/reportsubmission)**</span><span class="sxs-lookup"><span data-stu-id="7ccd3-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="7ccd3-108">Turvallisten lähettäjien käyttöä Outlookissa, Sallittujen lähettäjien  luetteloa tai sallittujen toimialueiden luetteloa roskapostin estokäytäntöjen avulla on vältettävä, koska lähettäjät ohittavat kaiken roskapostin, tekeutumisen ja tietojen lähettäjän suojauksen sekä lähettäjän todennuksen (SPF, DKIM, DMARC).</span><span class="sxs-lookup"><span data-stu-id="7ccd3-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="7ccd3-109">Tätä menetelmää käytetään parhaiten vain tilapäistesteissä.</span><span class="sxs-lookup"><span data-stu-id="7ccd3-109">This method is best used for temporary testing only.</span></span>
