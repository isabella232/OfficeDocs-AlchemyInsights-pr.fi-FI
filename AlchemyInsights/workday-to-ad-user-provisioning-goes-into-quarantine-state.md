---
title: Työpäivä AD-käyttäjien valmisteluun siirtyy karanteeniin
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
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481357"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Työpäivä AD-käyttäjien valmisteluun siirtyy karanteeniin

**Työpäivä AD-käyttäjien valmisteluun siirtyy karanteeniin eikä käyttäjiä luoda AD:ssä**

Työpäivä AD-käyttäjien valmistelutyö on mennyt karanteeniin, ja valvontalokeja käytettäessä näytetään vientivirhetapahtumat, joiden virhesanoma **on Virhe: OperationsError-SvcErr: Tapahtui toimintovirhe. Hakemistopalveluun ei ole määritetty parempia viittauksia. Hakemistopalvelu ei siis voi antaa suosituksia tämän metsän ulkopuolisille objekteille.** Tämä virhe ilmenee yleensä, jos Active Directory -säilöä OU ei ole määritetty oikein tai jos **parentDistinguishedName-lausekkeen yhdistämismäärityksessä on ongelmia.**

Tarkista uusien käyttäjien oletus ou **-parametri** kirjoitusvirheiden tarkistaminen. Varmista, että määritetty OU on jo ad-kentässä. Jos käytät **parentDistinguishedName-nimeä** määritteiden yhdistämisessä, varmista, että se arvioi aina AD-toimialueen tunnetun säilön. Tarkista valvontalokien Vie-tapahtuma, jotta näet luodun arvon.

Lisätietoja työpäivän määrittämisestä automaattista valmistelua varten on opetusohjelmassa: Työpäivän määrittäminen [automaattista käyttäjien valmistelua varten.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

