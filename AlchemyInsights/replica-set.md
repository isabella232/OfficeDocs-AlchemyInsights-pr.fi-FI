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
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110677"
---
# <a name="replica-set"></a>Replikointijoukko

AADDS tunnetaan myös hallituna toimialueena. Se on itse asiassa kaksi toimialueen ohjauskonetta, joita taustakone suorittaa ja ylläpitää. Kaksi DCs-tietokonetta sisältävät yhden dc:n päätietokoneen ja yhden replikoinnin DC:n. Varmuuskopiot AADDS:ssä (hallittu toimialue) ovat Azure-ympäristön hallitsemia automaattisia prosessia. Jos hallitussa toimialueessa ilmenee ongelma, Azure-tuki voi auttaa sinua palauttamaan varmuuskopion.

Luot kunkin replikointijoukon virtuaalisessa verkossa. Jokainen näennäisverkko on vertaisverkko kaikkiin muihin virtuaaliverkkoihin, jotka isännöidä hallitun toimialueen replikointijoukkoa. Tämä määritys luo verkkoverkkotopologian, joka tukee hakemiston replikointia. Virtuaalinen verkko voi tukea useita replikointijoukkoja, jos kukin replikointijoukko on eri virtuaalisessa aliverkossa.

Lisätietoja replikointijoukosta on kohdassa [Käsitteiden replikointijoukot.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)
