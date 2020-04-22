---
title: Ongelman vianmääritys - Käyttäjää ei löydy hakemistosta
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702735"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>Ongelman vianmääritys - Käyttäjää ei löydy hakemistosta

Jos käyttäjät saavat hakemistosta virhesanoman "käyttäjää ei löydy", yritä uudelleen, missä seurantakohteen tyyppi ei ole hakemistossa.

Seuraavat vaiheet voidaan suorittaa ongelman vianmäärityksen jälkeen.

- Varmista, että sähköpostikutsun hyväksynyt tili on sama tili, jota käytetään myöhemmin kirjautumiseen. Varmista, että käyttäjä käyttää samaa tiliä kutsuan hyväksymiseen ja kirjautumiseen sivustoon. 

Lisätietoja on [ohjeaiheessa Microsoft-tilin</a> aliasten hallinta Microsoft 365 -kirjautumisen hallintaa varten](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases). 

- Selaa jokaiseen sivustoon tai sivustoihin, joissa käyttäjä saa virheen. 

Lisää sivuston URL-osoitteen loppuun "/_layouts/15/people.aspx/membershipgroupid=0" (lainausmerkkien sisällä). 

Esimerkki: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.

- Valitse käyttäjä luettelosta.

- Valitse valintanauhasta **Poista käyttöoikeudet.** 
-  Lisää käyttäjä takaisin ja Lähetä kutsu uudelleen käyttäjälle.

