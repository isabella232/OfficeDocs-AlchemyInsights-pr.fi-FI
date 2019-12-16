---
title: Ongelman vian määritys-käyttäjää ei löydy hakemistosta
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0f1e427801107109e31486a4d300f53084880caf
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054807"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Ongelman vian määritys-käyttäjää ei löydy hakemistosta

Jos käyttäjät saavat virhe sanoman "käyttäjää ei löydy" hakemistosta, yritä uudelleen, jos ongelma tyyppi on käyttäjä ei ole hakemistoon.

Seuraavat vaiheet voidaan suorittaa ongelman vian määritystä varten.

- Varmista, että sähkö posti kutsun hyväksynyt tili on sama tili, jota käytetään kirjautumiseen myöhemmin. Varmista, että käyttäjä käyttää samaa tiliä hyväksyäksesi kutsun ja kirjautumiseen sivustoon. 

Lisä tietoja on Ohje aiheessa [Microsoft-tilin</a> tunnusten hallinta Office 365-kirjautumistietojen hallintaa](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)varten. 

- Selaa jokaiseen sivustoon, jossa käyttäjä saa virheen. 

Lisää "/_layouts/15/People.aspx/membershipgroupid = 0" (lainaus merkkien sisällä) sivuston URL-osoitteen loppuun. 

Esimerkki: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Valitse käyttäjä luettelosta.

- Valitse **Poista käyttö oikeudet** valinta nauhasta. 
-  Lisää käyttäjä takaisin ja Lähetä kutsu käyttäjälle uudelleen.

