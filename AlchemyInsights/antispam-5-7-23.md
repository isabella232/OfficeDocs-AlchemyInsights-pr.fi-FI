---
title: Antispam-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682116"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Korjaa sähkö postin toimitus ongelmat virhe koodilla 5.7.23

Tarkista verkko tunnuksesi SPF DNS-tietue julkisesti saatavilla olevalla SPF-tai DNS-tietueen tarkistus sivulla verkossa.

Varmista, että Office 365 ei tunnistanut lähtevää viestiä roska postiksi ja että se on reititetty [suuren riskin toimitus varannon](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages)kautta. Suuren riskin toimitus varannon viestit eivät läpäise SPF-tarkastuksia, joten kohde Sähkö posti organisaatio ei hyväksy niitä.

Jos ongelma jatkuu, sinun on ehkä otettava yhteyttä Sähkö posti isännän ylläpitäjään, johon yrität lähettää sähkö postia. Merkitse heijastus viestissä käytettävissä oleva yksityiskohtainen ulkoinen virhe.  Office 365-tuki ei välttämättä pysty auttamaan.