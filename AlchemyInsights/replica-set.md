---
title: Replikointijoukko
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50713748"
---
# <a name="replica-set"></a>Replikointijoukko

AADDS tunnetaan myös hallituna toimialueena. Se on itse asiassa kaksi toimialueen ohjauskonetta, joita taustaohjain suorittaa ja ylläpitää. Nämä kaksi DCs-tietokonetta sisältävät yhden dc:n päätietokoneen ja yhden replikoinnin DC:n. Varmuuskopiot AADDS:ssä (hallittu toimialue) ovat Azure-ympäristön hallitsemia automaattisia prosessia. Jos hallittuun toimialueeseen liittyy ongelma, Azuren tuki auttaa sinua palauttamaan tiedot varmuuskopioista.

Jokainen replikointijoukko luodaan virtuaalisessa verkossa. Kunkin virtuaalisen verkoston on oltava vertaisverkko kaikissa muissa virtuaaliverkoissa, joissa isännöidä hallitun toimialueen replikointijoukkoa. Tämä määritys luo verkkotopologian, joka tukee hakemiston replikointia. Virtuaalinen verkko voi tukea useita replikointijoukkoja, jos kukin replikointijoukko on eri virtuaalisessa aliverkossa.

Lisätietoja replikointijoukosta on konseptien [replikointijoukoissa.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
