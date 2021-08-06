---
title: Työpäivä AD-käyttäjien valmisteluun siirtyy karanteenitilaksi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036489"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Työpäivä AD-käyttäjien valmisteluun siirtyy karanteenitilaksi

**Työpäivä AD-käyttäjien valmisteluun siirtyy karanteenitilaksi eikä käyttäjiä luoda AD:ssä**

Workday to AD User Provisioning -työ on viety karanteeniin ja valvontalokeja käytettäessä näytetään vientivirhetapahtumat, joiden virhesanomana on **Virhe: OperationsError-SvcErr: Tapahtui toimintovirhe. Hakemistopalvelua varten ei ole määritetty ylivertaista viittausta. Hakemistopalvelu ei siis voi antaa suosituksia tämän metsän ulkopuolisille objekteille.** Tämä virhe ilmenee yleensä, jos Active Directory -säilön OU-määritystä ei ole määritetty oikein tai **parentDistinguishedName-lausekkeen yhdistämisessä on ongelmia.**

Tarkista kirjoitusvirheitä oletus OU **uusille käyttäjille** -parametrista. Varmista, että määritetty OU on jo AD:ssä. Jos käytät **määritemäärityksessä parentDistinguishedName-nimeä,** varmista, että se arvioi aina AD-toimialueen tunnetun säilön. Tarkista luotu arvo valvontalokien Vie-tapahtumasta.

Lisätietoja automaattisen valmistelun työpäivän määrittämisestä on kohdassa [Opetusohjelma: Työpäivän määrittäminen automaattista käyttäjien valmistelua varten.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

