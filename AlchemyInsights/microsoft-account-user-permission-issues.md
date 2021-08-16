---
title: Vianmääritysongelma – käyttäjää ei löydy hakemistosta
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 79429f8e9523ad6b08cd2cd2b19dd221bac797d00de142cbb18826b86fb5ae4e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098167"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Vianmääritysongelma – käyttäjää ei löydy hakemistosta

Jos käyttäjät saavat hakemistosta virheilmoituksen "käyttäjää ei löydy", yritä uudelleen kohtaa, jossa Ongelman tyyppi on Käyttäjä ei ole hakemistossa.

Voit suorittaa ongelman vianmäärityksen seuraavien vaiheiden avulla.

- Varmista, että sähköpostikutsun hyväksynnyllä tilillä on sama tili, jota käytetään myöhemmin kirjautumaan sisään. Varmista, että käyttäjä hyväksyy kutsun ja kirjautuu sivustoon käyttämällä samaa tiliä. 

Lisätietoja on kohdassa [Microsoft-tilin aliaksien hallinta kirjautumisen </a> Microsoft 365.](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases) 

- Siirry kaikkiin sivustoihin, joissa käyttäjä saa virheilmoituksen. 

Lisää "/_layouts/15/people.aspx/membershipgroupid=0" (lainausmerkeissä) sivuston URL-osoitteen loppuun. 

Esimerkki: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Valitse käyttäjä luettelosta.

- Valitse **valintanauhasta Poista** käyttöoikeudet. 
-  Lisää takaisin käyttäjä ja lähetä kutsu uudelleen käyttäjälle.

