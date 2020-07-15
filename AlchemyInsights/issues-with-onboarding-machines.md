---
title: Perehdytyskoneisiin liittyvät ongelmat
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141466"
---
# <a name="issues-with-onboarding-machines"></a>Perehdytyskoneisiin liittyvät ongelmat

MDATP-palveluun liittyvissä koneiden käytössä saattaa olla ongelmia. Jos voit käyttää loppukäyttäjäkonetta, toimi seuraavasti:

1. Lataa [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) -diagnostiikkatyökalu.
2. Pura ja suorita MDATPAnalyzer.cmd.
3. Etsi diagnostiikkaloki kansiosta nimeltä MDATPClientAnalyzerResult, samasta kansiosta, johon Analyzer-työkalu ladataan.
4. Tarkista lokitiedostosta MDATPClientAnalyzer.txt yhteys- tai internet-välityspalvelimen asetukset.