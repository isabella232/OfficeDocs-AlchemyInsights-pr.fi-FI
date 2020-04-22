---
title: Lähtevä sähköposti Roskaposti-kansioon
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 2350586e95f316061ff855d152e86db0547eb209
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761165"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="fcf8e-102">Lähtevä sähköposti Roskaposti-kansioon</span><span class="sxs-lookup"><span data-stu-id="fcf8e-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="fcf8e-103">Jos näet lähtevien viestien merkitsemisen roskapostiksi, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="fcf8e-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="fcf8e-104">Jos et ole vielä määrittänyt [lähtevien roskapostiilmoitusten määrittämistä](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="fcf8e-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="fcf8e-105">[Viestin jäljityksen](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) avulla voit tarkistaa, onko lähtevän viestin tapahtumaarvo **Roskaposti** ja lisätiedot: Käytä suuren **riskin toimituspoolia**.</span><span class="sxs-lookup"><span data-stu-id="fcf8e-105">Use [message trace](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="fcf8e-106">Tarkista näiden viestien sisällöstä, mitä voidaan pitää roskapostina.</span><span class="sxs-lookup"><span data-stu-id="fcf8e-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="fcf8e-107">Allekirjoitukset voivat esimerkiksi joskus aiheuttaa ongelmia monille käyttäjille.</span><span class="sxs-lookup"><span data-stu-id="fcf8e-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="fcf8e-108">Jos sinulla on useita esimerkkejä laillisista lähtevistä viesteistä, jotka on merkitty roskapostiksi, avaa tukipyyntö ja pyydä tukiagenttia lähettämään viestisi väärinä positiivisina roskapostianalyytikoillemme.</span><span class="sxs-lookup"><span data-stu-id="fcf8e-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="fcf8e-109">Valmistaudu antamaan malliviestejä, jotka sisältävät kaikki viestin otsikot.</span><span class="sxs-lookup"><span data-stu-id="fcf8e-109">Be prepared to provide sample messages that include all message headers.</span></span>
