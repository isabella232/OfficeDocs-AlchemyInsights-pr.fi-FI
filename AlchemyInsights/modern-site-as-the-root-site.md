---
title: Kuin pääsivusto nykyaikaisia sivusto
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 260048db6c439183da8e0bb0c2dfa3c7475fca79
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/09/2019
ms.locfileid: "36269373"
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
