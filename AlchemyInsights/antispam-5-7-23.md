---
title: Roska postin esto-5.7.23
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
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717322"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>Sähkö postin välitys ongelmien korjaaminen virhe koodissa 5.7.23

Varmista, että toimi alueesi SPF DNS-tietue on julkisesti saatavilla olevassa SPF-tai DNS-tietueiden tarkistuksessa verkossa.

Varmista, että Microsoft ei ole määrittänyt lähtevää viestiä roska postiksi, ja reititetty [suuren riskin lähetys varannon](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)kautta. Suuren riskin vastaanotto varannon viestit eivät läpäise SPF-tarkistuksia, joten kohde Sähkö posti organisaatio ei hyväksy niitä.

Jos ongelma jatkuu, sinun on ehkä otettava yhteyttä sen Sähkö posti palvelimen järjestelmänvalvojaan, johon yrität lähettää sähkö postia. Merkitse muistiin palautus viestissä oleva tarkka ulkoinen virhe. Microsoft-tuki ei ehkä pysty auttamaan.
