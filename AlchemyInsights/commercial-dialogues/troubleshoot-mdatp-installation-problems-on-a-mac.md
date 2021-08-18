---
title: MDATP-asennusongelmien vianmääritys Macissa
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091025"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>MDATP-asennusongelmien vianmääritys Macissa

Jos manuaalinen asennus epäonnistuu, **ohjatun** asennuksen yhteenvetosivulla näkyy seuraava virhe:

"Asennuksen aikana tapahtui virhe. Asennusohjelma kohtasi virheen, joka aiheutti asennuksen epäonnistumisen. Pyydä apua ohjelmistovalmistajalta."

MDM-käyttöönotoissa sivulla näkyy myös yleinen asennusvirhe.

Vaikka loppukäyttäjät eivät näytä tarkkoja virheitä, säilytämme asennuksen edistymisen lokitiedoston **kohteessa /Library/Logs/Microsoft/mdatp/install.log**. Jokainen asennusistunto liitetään tähän lokitiedostoon. Jos haluat käyttää vain viimeistä asennusistuntoa, käytä `sed` -

Lisätietoja on kohdassa [Microsoft Defender ATP for Macin asennusongelmien vianmääritys.](https://go.microsoft.com/fwlink/?linkid=2144615)
