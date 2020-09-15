---
title: Active Directory ei synkronoidu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697626"
---
# <a name="active-directory-not-syncing"></a>Active Directory ei synkronoidu

Jos saat synkronointi virheitä, kuten "ei hiljattain tehtyä synkronointia" tai huomaat, että Office-hallinta portaalin hakemisto synkronoinnin tilana lukee "synkronoitu viimeksi yli 3 päivää sitten", voi olla, että AADConnect-asetukset ovat virheelliset tai käyttö oikeudet eivät riitä synkronoinnin suorittamiseen.  

AADConnect-toiminnon uudelleenasentaminen Pika-asetuksilla voi korjata ongelman nopeasti:

1. [Lataa AADConnect-tiedoston uusin versio](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Noudata pika-asennus ohjeita](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Lisä tietoja AADConnect-palvelu tileiltä on Ohje aiheessa [Azure AD Connect: Asiakkaat ja käyttö oikeudet](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
