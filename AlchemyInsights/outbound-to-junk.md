---
title: Lähtevä Sähkö posti roska posti-kansioon
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 371d2c46e9048365fd343145330536bd9cf1db82
ms.sourcegitcommit: 1002f510fadb92c143cd6bbb60b42a851d5a38e1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/20/2019
ms.locfileid: "37062768"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="905ea-102">Lähtevä Sähkö posti roska posti-kansioon</span><span class="sxs-lookup"><span data-stu-id="905ea-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="905ea-103">Jos näet, että lähtevät viestit merkitään roska postiksi, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="905ea-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="905ea-104">Harkitse [lähtevien roska posti käytäntöjen ilmoitusten määrittämistä](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy), jos et ole jo tehnyt niin.</span><span class="sxs-lookup"><span data-stu-id="905ea-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/office365/securitycompliance/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="905ea-105">Käytä [Sanomien jäljitystä](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) nähdäksesi, onko lähtevässä viestissä tapahtuma arvo **roska posti** , jossa on lisä tietoja: **Käytä suuren riskin toimitus varannon**.</span><span class="sxs-lookup"><span data-stu-id="905ea-105">Use [message trace](https://docs.microsoft.com/office365/securitycompliance/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="905ea-106">Jos kyse on näistä viesteistä, tarkista viestin sisältö ja Katso, mitä roska postiksi saatetaan pitää.</span><span class="sxs-lookup"><span data-stu-id="905ea-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="905ea-107">Esimerkiksi allekirjoitukset voivat joskus aiheuttaa ongelmia monille käyttäjille.</span><span class="sxs-lookup"><span data-stu-id="905ea-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="905ea-108">Jos sinulla on useita esimerkkejä laillisista lähtevistä viesteistä, jotka on merkitty roska postiksi, avaa tuki pyyntö ja pyydä tuki agenttia lähettämään viestisi vääriksi positiivisiksi roska postin analyytikoille.</span><span class="sxs-lookup"><span data-stu-id="905ea-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="905ea-109">Valmistaudu tarjoamaan näyte sanomia, jotka sisältävät kaikki viestien otsikot.</span><span class="sxs-lookup"><span data-stu-id="905ea-109">Be prepared to provide sample messages that include all message headers.</span></span>
