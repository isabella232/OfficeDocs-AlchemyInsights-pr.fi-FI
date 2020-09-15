---
title: 'Virhe: tämän tieto koneen säännöt eivät täsmää'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690960"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="a2866-102">Virhe: tämän tieto koneen säännöt eivät täsmää</span><span class="sxs-lookup"><span data-stu-id="a2866-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="a2866-103">Jos haluat nähdä tämän tunnetun ongelman päivitetyn tilan, katso [tämän tieto koneen säännöt eivät vastaa Microsoft Exchangen sääntöjä](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0) .</span><span class="sxs-lookup"><span data-stu-id="a2866-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="a2866-104">Outlook-tiimi on toteuttanut korjaus tiedoston koonti versio 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="a2866-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="a2866-105">Korjaus on jo Insider Fast-ohjelmassa ja se siirtyy kuukausi kanavaan 2020 kesä kuun lopulla.</span><span class="sxs-lookup"><span data-stu-id="a2866-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="a2866-106">Kun sinulla on korjattu koonti versio, näyttöön voi tulla kehote "mitä sääntöjä haluat säilyttää".</span><span class="sxs-lookup"><span data-stu-id="a2866-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="a2866-107">Valitse palvelin pyydettäessä ja palaa sitten Outlook-ohjelmassa uudelleen ja ota käyttöön kaikki käytöstä poistetut säännöt.</span><span class="sxs-lookup"><span data-stu-id="a2866-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="a2866-108">Ennen kuin korjaus on käytettävissä, käytä seuraavaa vaihto ehtoista menetelmää:</span><span class="sxs-lookup"><span data-stu-id="a2866-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="a2866-109">**Vaihtoehtoinen**menetelmä: Viimeaikaiset raportit ovat aiheuttaneet ongelman niille, jotka ovat luoneet vain asiakas sääntöjä Outlookin Työpöytä versiossa.</span><span class="sxs-lookup"><span data-stu-id="a2866-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="a2866-110">Jos ongelma jatkuu edelleen, kannattaa harkita sääntöjen poistamista ja luoda ja muokata sääntöjä vain OWA (Outlook Web App)-sovelluksessa, ennen kuin ongelma on ratkaistu.</span><span class="sxs-lookup"><span data-stu-id="a2866-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="a2866-111">Jos et voi poistaa sääntöjä manuaalisesti, voit suorittaa Outlook-komennon, kun käynnistät Outlookin suorittamalla Outlook.exe/cleanrules.</span><span class="sxs-lookup"><span data-stu-id="a2866-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="a2866-112">Tämä toiminto poistaa sekä asiakas-että palvelin säännöt.</span><span class="sxs-lookup"><span data-stu-id="a2866-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="a2866-113">Se poistaa kaikki säännöt kaikille Outlook-profiilissa oleville tileille.</span><span class="sxs-lookup"><span data-stu-id="a2866-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="a2866-114">Tämä komento on edelleen dokumentoitu komento rivi valitsimien artikkelissa.</span><span class="sxs-lookup"><span data-stu-id="a2866-114">This command is further documented in the Command-line switches article.</span></span>

