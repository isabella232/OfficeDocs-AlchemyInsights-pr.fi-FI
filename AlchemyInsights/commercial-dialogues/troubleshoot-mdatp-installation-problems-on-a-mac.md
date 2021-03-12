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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746305"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>MDATP-asennusongelmien vianmääritys Macissa

Jos manuaalinen asennus epäonnistuu, **ohjatun** asennuksen yhteenvetosivulla näkyy seuraava virhe:

"Asennuksen aikana tapahtui virhe. Asennusohjelma kohtasi virheen, joka aiheutti asennuksen epäonnistumisen. Pyydä apua ohjelmistovalmistajalta."

MDM-käyttöönotoissa sivulla näkyy myös yleinen asennusvirhe.

Vaikka emme näytä tarkkoja virheitä loppukäyttäjille, säilytämme lokitiedoston asennuksen edistymisen kanssa **kohteessa /Library/Logs/Microsoft/mdatp/install.log.** Jokainen asennusistunto liitetään tähän lokitiedostoon. Jos haluat tulostaa vain viimeisen asennusistunnon, käytä `sed` .

Lisätietoja on kohdassa [Microsoft Defender ATP for Macin asennusongelmien vianmääritys.](https://go.microsoft.com/fwlink/?linkid=2144615)
