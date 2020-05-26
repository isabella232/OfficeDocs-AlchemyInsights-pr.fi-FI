---
title: Ryhmien kirjautumisvirheen käsitteleminen AADSTS9000411
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: b70f1320ea1dfa29e6fa489bd02acfcd1d92971b
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357550"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="7214d-102">Ryhmien kirjautumisvirheen käsitteleminen AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="7214d-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="7214d-103">Kun kirjaudut Microsoft Teamsiin, näyttöön saattaa tulla virhe: **Valitettavasti sinulla on ongelmia kirjautumisessa AADSTS9000411: Pyyntöä ei ole muotoiltu oikein. Parametri "login_hint" on monistettu.**</span><span class="sxs-lookup"><span data-stu-id="7214d-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="7214d-104">Voit korjata tämän ongelman varmistamalla, että Microsoft Teams -asiakkaasi päivitetään.</span><span class="sxs-lookup"><span data-stu-id="7214d-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="7214d-105">Lisätietoja asiakkaan päivittämisestä on ohjeaiheessa [Microsoft Teamsin päivittäminen](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="7214d-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="7214d-106">Jos asiakasohjelmaa ei jostain syystä voi päivittää, asiakkaan uloskirjautuminen tyhjentää useimmat välimuistissa olevat tiedot.</span><span class="sxs-lookup"><span data-stu-id="7214d-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="7214d-107">Jos sinulla on kuitenkin ongelmia uloskirjautumisen/kirjautumisen jälkeen, sulje Teams ja tyhjennä asiakasvälimuisti seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="7214d-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="7214d-108">Sulje Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="7214d-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="7214d-109">Siirry kohtaan: %appdata%\microsoft\teams ja poista kaikki tiedostot.</span><span class="sxs-lookup"><span data-stu-id="7214d-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="7214d-110">Avaa Microsoft Teams uudelleen.</span><span class="sxs-lookup"><span data-stu-id="7214d-110">Reopen Microsoft Teams.</span></span>
