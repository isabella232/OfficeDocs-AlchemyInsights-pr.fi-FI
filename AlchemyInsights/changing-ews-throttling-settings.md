---
title: Muutetaan EWS-rajoitusasetuksia
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
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 16916d5f16f763d87ce0d5ef830e741279c9f4df
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818033"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="7c23d-102">Muutetaan EWS-rajoitusasetuksia</span><span class="sxs-lookup"><span data-stu-id="7c23d-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="7c23d-103">Suorita automaattinen testimme, jonka avulla voit muuttaa EWS-rajoituskäytäntöä siirron ajaksi.</span><span class="sxs-lookup"><span data-stu-id="7c23d-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="7c23d-104">Huomaa, että testin suorituksenkin jälkeen, EWS-tuonnit on silti rajoitettu 150 megatavuun 5 minuutin sisällä postilaatikkoa kohti. Jos haluat saavuttaa korkeammat siirtonopeudet, siirrä useampia käyttäjiä samanaikaisesti.</span><span class="sxs-lookup"><span data-stu-id="7c23d-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="7c23d-105">Huomaa, että EWS-rajoituskäytännön muutoksilla ei ole vaikutusta seuraaviin siirtotyyppeihin (Microsoft-työkaluja käytettäessä): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Yleinen kansio tai PST-tuontipalvelu.</span><span class="sxs-lookup"><span data-stu-id="7c23d-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>