---
title: Ongelman vian määritys-käyttäjää ei löydy hakemistosta
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725404"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Ongelman vian määritys-käyttäjää ei löydy hakemistosta

Jos käyttäjät saavat virhe ilmoituksen "käyttäjää ei löydy" hakemistosta, yritä uudelleen, kun ongelma tyyppi on käyttäjä, joka ei ole hakemistossa.

Voit suorittaa ongelman vian määrityksen suorittamalla seuraavat vaiheet.

- Varmista, että sähkö posti kutsun hyväksynyt tili on sama tili, jota käytetään kirjautumiseen myöhemmin. Varmista, että käyttäjä käyttää samaa tiliä, jotta voit hyväksyä kutsun ja kirja utua sivustoon. 

Lisä tietoja on Ohje aiheessa Microsoft- [Tilin aliaksien hallinta </a> Microsoft 365-kirjautumisen hallintaa](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)varten. 

- Selaa jokaiseen sivustoon, jossa käyttäjä saa virhe ilmoituksen. 

Lisää "/_layouts/15/People.aspx/membershipgroupid = 0" (lainaus merkkien sisällä) sivuston URL-osoitteen loppuun. 

Esimerkki: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Valitse käyttäjä luettelosta.

- Valitse valinta nauhasta **Poista käyttö oikeudet** . 
-  Lisää käyttäjä takaisin ja Lähetä kutsu käyttäjälle uudelleen.

