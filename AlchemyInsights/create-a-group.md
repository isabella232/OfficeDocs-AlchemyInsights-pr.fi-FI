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
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816345"
---
# <a name="create-a-group"></a>Ryhmän luominen

Tässä ohjeaiheessa kerrotaan ryhmien luomisesta.

**Ryhmän luontioikeus**

Varmista, että sinulla on oikeus luoda uusi ryhmä. Yleiset järjestelmänvalvojat voivat poistaa käytöstä ryhmien luomisen Azure-portaalissa tai käyttöpaneelissa. Tarvitset ehkä järjestelmänvalvojan, jotta voit luoda uuden ryhmän, tai antaa sinulle tarvittavat käyttöoikeudet.

**Ryhmän luontioikeuksien hallinta**

1. Yleiset järjestelmänvalvojat voivat hallita ryhmien luontioikeuksia (tietoturvasyistä) tai Azure-portaalissa tai -paneelissa luotuja Office 365 -ryhmiä valitsemalla Käyttäjät voivat luoda käyttöoikeusryhmiä Azure-portaaleissa tai Käyttäjät voivat luoda Office 365 -ryhmiä Azure-portaaleissa -vaihtoehdot Kaikki ryhmät Yleiset   >  **(Asetukset)**-kohdassa.
2. Voit myös rajoittaa ryhmien luomisen valitsemaan käyttäjäryhmän, jos sinulla on Azure Active Directory P1 Premium -käyttöoikeus.

**Tervetuloilmoituksen poistaminen käytöstä uusille Office 365 -ryhmän jäsenille**

Office 365 -ryhmiin lisätyille käyttäjille lähetettävä tervetuloilmoitus voidaan poistaa käytöstä määrittämällä **UnifiedGroupWelcomeMessageEnabled-arvoksi** Epätosi Powershellissä. Lisätietoja tästä [asetuksesta on täällä](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

