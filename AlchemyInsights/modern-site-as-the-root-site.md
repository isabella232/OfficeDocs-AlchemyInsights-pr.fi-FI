---
title: Kuin pääsivusto nykyaikaisia sivusto
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1874"
- "9000265"
ms.openlocfilehash: b30fc3258bb76c0ab4bf10af0ec9317417f7c663
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232712"
---
# <a name="modern-site-as-root-site"></a>Kuin pääsivusto nykyaikaisia sivusto

Emme ole aloittaneet rahoittaja on uusi ominaisuus, joka mahdollistaa perinteinen sivuston pääkansio sivustosi Moderni sivuston kanssa vaihdettava. [Invoke-SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) avulla sivuston toisen sivuston kanssa vaihdettava tallennettaessa alkuperäiseen sivustoon. Sekä ryhmän (ei yhteyttä ryhmään) ja tiedonannon sivustojen käytettävissä. 

>[!Important]
> Älä poista perinteinen pääsivusto luoda Nykyaikainen Viestimissivusto. Microsoft ei tue. Ensisijaisen säilön poistaminen tekee kaikki SharePoint-sivustot organisaation kaikkien käyttäjien käytettävissä ennen kuin palauttaa sivuston tai luoda uuden sivuston samaan URL-osoitteeseen. Olemme yhteydessä tämän toiminnon kautta viestikeskus. Tulee odottaa-ominaisuuden avulla voidaan ottaa käyttöön oman vuokralaisen pian.

## <a name="known-issues-with-swapping-sites"></a>Tunnettuja ongelmia vaihtamisen sivustot
- Kohdesivuston saattaa palauttaa (HTTP 404) ”ei löydy” virhe lyhyen ajan kuluessa.
- Sisältöä täytyy päivittää hakuindeksin tehdään uudelleen. Ei ole pakollinen tässä kentässä Manuaalinen vaihe, tämä tapahtuu automaattisesti.
- Mitään riippuvainen ”staattinen” linkkejä (kuten tiedoston synkronointiin ja OneNote-tiedostoja) on korjattava manuaalisesti.
- Project Server-sivustoja on ehkä tarkistettava sen varmistamiseksi, että ne liittyvät yhä oikein. 
