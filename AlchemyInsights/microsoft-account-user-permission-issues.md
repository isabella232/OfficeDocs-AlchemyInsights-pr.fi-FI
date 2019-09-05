---
title: Ongelman vian määritys-käyttäjää ei löydy hakemistosta
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81b9dafe8e27e5f73fe232c51ff56fed3fec29b4
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36754189"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Ongelman vian määritys-käyttäjää ei löydy hakemistosta

Jos käyttäjät saavat virhe sanoman "käyttäjää ei löydy" hakemistosta. Yritä uudelleen, jos ongelma tyyppi on käyttäjä, joka ei ole kansiossa.

Seuraavat vaiheet voidaan suorittaa ongelman vian määritystä varten.

- Varmista, että sähkö posti kutsun hyväksynyt tili on sama tili, jota käytetään kirjautumiseen myöhemmin. Varmista, että käyttäjä käyttää samaa tiliä hyväksyäksesi kutsun ja kirjautumiseen sivustoon. 

Lisä tietoja on Ohje aiheessa [Microsoft-tilin</a> tunnusten hallinta Office 365-kirjautumistietojen hallintaa](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)varten. 

- Selaa jokaiseen sivustoon, jossa käyttäjä saa virheen. 

Lisää "/_layouts/15/People.aspx/membershipgroupid = 0" (lainaus merkkien sisällä) sivuston URL-osoitteen loppuun. 

Esimerkki: https://_LT_ "contoso">. SharePoint. com/_asettelut/15/People. aspx/membershipGroupId = 0.

- Valitse käyttäjä luettelosta.

- Valitse **Poista käyttö oikeudet** valinta nauhasta. 
-  Lisää käyttäjä takaisin ja Lähetä kutsu käyttäjälle uudelleen.

