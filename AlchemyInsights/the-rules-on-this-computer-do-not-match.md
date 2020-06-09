---
title: 'Virhe: Tämän tietokoneen säännöt eivät vastaa toisiaan'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: ecc1e5ec741cc90c58698991c3a3135f87c39938
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/09/2020
ms.locfileid: "44617966"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="ce99e-102">Virhe: Tämän tietokoneen säännöt eivät vastaa toisiaan</span><span class="sxs-lookup"><span data-stu-id="ce99e-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="ce99e-103">Lisätietoja tämän tunnetun ongelman päivitetystä tilasta on [ohjeaiheessa Tämän tietokoneen säännöt eivät vastaa Microsoft Exchangen sääntöjä.](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="ce99e-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="ce99e-104">Outlook-tiimi on ottanut käyttöön korjauksen koontiversiossa 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="ce99e-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="ce99e-105">Korjaus on jo Insider Fast ja menee Monthly Channel kesäkuun lopulla 2020.</span><span class="sxs-lookup"><span data-stu-id="ce99e-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="ce99e-106">Kun olet kiinteä rakentaa saatat saada kehotteen "Mitkä säännöt haluat pitää" viimeisen kerran.</span><span class="sxs-lookup"><span data-stu-id="ce99e-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="ce99e-107">Valitse Pyydettäessä Palvelin ja palaa sitten Outlookiin ja ota käytöstä poistetut säännöt uudelleen käyttöön.</span><span class="sxs-lookup"><span data-stu-id="ce99e-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="ce99e-108">Ennen kuin korjaus on saatavilla, käytä seuraavaa kiertotapaa:</span><span class="sxs-lookup"><span data-stu-id="ce99e-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="ce99e-109">**Vaihtoehtoinen menetelmä:** Viimeaikaisissa raporteissa ongelma on ilmennyt niille, jotka ovat luoneet asiakassääntöjä vain Outlook-työpöydällä.</span><span class="sxs-lookup"><span data-stu-id="ce99e-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="ce99e-110">Jos ongelma jatkuu, harkitse sääntöjen poistamista ja sääntöjen luomista ja muokkaamista vain OWA:ssa (Outlook Web App), kunnes ongelma on ratkaistu.</span><span class="sxs-lookup"><span data-stu-id="ce99e-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="ce99e-111">Jos et voi poistaa sääntöjä manuaalisesti, voit suorittaa Outlook-komennon, kun käynnistät Outlookin suorittamalla Outlook.exe /cleanrules-ohjelman.</span><span class="sxs-lookup"><span data-stu-id="ce99e-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="ce99e-112">Tämä poistaa sekä asiakas- että palvelinsäännöt.</span><span class="sxs-lookup"><span data-stu-id="ce99e-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="ce99e-113">Se poistaa kaikki säännöt kaikille tileille Outlook-profiilissa.</span><span class="sxs-lookup"><span data-stu-id="ce99e-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="ce99e-114">Tämä komento on edelleen dokumentoitu Komentorivivalitsit -artikkelissa.</span><span class="sxs-lookup"><span data-stu-id="ce99e-114">This command is further documented in the Command-line switches  article.</span></span>