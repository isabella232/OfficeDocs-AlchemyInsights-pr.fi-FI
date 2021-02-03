---
title: Muutetaan EWS-rajoitusasetuksia
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
- "9000752"
- "5653"
- "5760"
ms.openlocfilehash: 4f0bea884153dc1ed8699ce12e0d017d18f5e57c
ms.sourcegitcommit: 53e5caab697ebfb434ccef3ef98b8f2bee579b41
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/02/2021
ms.locfileid: "50075894"
---
# <a name="changing-ews-throttling-settings"></a><span data-ttu-id="f848c-102">Muutetaan EWS-rajoitusasetuksia</span><span class="sxs-lookup"><span data-stu-id="f848c-102">Changing EWS throttling settings</span></span>

<span data-ttu-id="f848c-103">Suorita automaattinen testimme, jonka avulla voit muuttaa EWS-rajoituskäytäntöä siirron ajaksi.</span><span class="sxs-lookup"><span data-stu-id="f848c-103">Please run our automated test which will allow you to modify the EWS throttling policy for the duration of your migration.</span></span> <span data-ttu-id="f848c-104">Huomaa, että suorituksen jälkeen, EWS-tuonnit on silti rajoitettu 150 megatavuun 5 minuutin sisällä per postilaatikko. Jos haluat saavuttaa korkeammat siirtonopeudet, siirrä useampia käyttäjiä samanaikaisesti.</span><span class="sxs-lookup"><span data-stu-id="f848c-104">Note that even after this is run, EWS imports will still be limited to 150mb per 5 minutes per mailbox; to achieve higher migration throughput speeds, please migrate more users concurrently.</span></span>

<span data-ttu-id="f848c-105">Huomaa, että EWS-rajoituskäytännön muutoksilla ei ole vaikutusta seuraaviin siirtotyyppeihin (Microsoft-työkaluja käytettäessä): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Yleinen kansio tai PST-tuontipalvelu.</span><span class="sxs-lookup"><span data-stu-id="f848c-105">Please note that EWS throttling policy changes have no effect on the following migration types (using Microsoft tools): Hybrid, Cutover/Staged (RPC/HTTP), IMAP, G Suite, Public Folder or PST Import Service.</span></span>