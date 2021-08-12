---
title: Ryhmän luominen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929302"
---
# <a name="create-a-group"></a>Ryhmän luominen

Tässä ohjeaiheessa kerrotaan ryhmien luomisesta.

**Ryhmän luontioikeus**

Varmista, että sinulla on oikeus luoda uusi ryhmä. Yleiset järjestelmänvalvojat voivat poistaa käytöstä ryhmien luomisen Azure-portaalissa tai käyttöpaneelissa. Tarvitset ehkä järjestelmänvalvojan, jotta voit luoda uuden ryhmän, tai antaa sinulle tarvittavat käyttöoikeudet.

**Ryhmän luontioikeuksien hallinta**

1. Yleiset järjestelmänvalvojat voivat hallita ryhmien luontioikeuksia (tietoturvasyistä) tai Office 365-ryhmiä, jotka on luotu Azure-portaalissa tai käyttöoikeuspaneelissa, valitsemalla "Käyttäjät voivat luoda käyttöoikeusryhmiä Azure-portaaleissa" tai "Käyttäjät voivat luoda Office 365-ryhmiä Azure-portaaleissa" -vaihtoehdon Kaikki ryhmät Yleiset  >  **(Asetukset)**-kohdassa.
2. Voit myös rajoittaa ryhmän luomisen ja valita käyttäjäryhmän, jos sinulla on Azure Active Directory P1-Premium käyttöoikeus.

**Tervetuloilmoituksen poistaminen käytöstä Office 365 ryhmän jäsenille**

Office 365-ryhmiin lisätyille käyttäjille lähetettävä tervetuloilmoitus voidaan poistaa käytöstä määrittämällä **UnifiedGroupWelcomeMessageEnabled-asetukseksi** Epätosi Powershellissä. Lisätietoja tästä [asetuksesta on täällä](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

