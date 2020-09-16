---
title: Lähtevän sähkö postin lähettäminen roska posti-kansioon
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769180"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="6531d-102">Lähtevän sähkö postin lähettäminen roska posti-kansioon</span><span class="sxs-lookup"><span data-stu-id="6531d-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="6531d-103">Jos näet lähtevät viestit, jotka on merkitty roska postiksi, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="6531d-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="6531d-104">Jos et ole vielä tehnyt sitä, harkitse [lähtevien roska posti käytäntöjen ilmoitusten määrittämistä](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="6531d-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="6531d-105">Käytä [viestin seurantaa](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) , jos haluat nähdä, onko lähtevän viestin tapahtuma-arvo **roska posti** , jossa on lisä tietoja: **Käytä suuren riskin lähetys allasta**.</span><span class="sxs-lookup"><span data-stu-id="6531d-105">Use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="6531d-106">Jos kyseessä on tämä viesti, tarkista viestin sisältö ja Katso, mitä roska postiksi voidaan pitää.</span><span class="sxs-lookup"><span data-stu-id="6531d-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="6531d-107">Esimerkiksi allekirjoitukset voivat toisinaan aiheuttaa ongelmia useille käyttäjille.</span><span class="sxs-lookup"><span data-stu-id="6531d-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="6531d-108">Jos sinulla on useita esimerkkejä oikeutetuista lähtevistä viesteistä, jotka on merkitty roska postiksi, avaa tuki pyyntö ja pyydä tuki henkilöä lähettämään viestisi epätodeksi roska postin analyytikoille.</span><span class="sxs-lookup"><span data-stu-id="6531d-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="6531d-109">Valmistaudu esittämään malli viestejä, jotka sisältävät kaikki viestin otsikot.</span><span class="sxs-lookup"><span data-stu-id="6531d-109">Be prepared to provide sample messages that include all message headers.</span></span>
