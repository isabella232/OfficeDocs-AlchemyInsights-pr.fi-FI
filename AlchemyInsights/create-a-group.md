---
title: Ryhmän luominen
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
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088690"
---
# <a name="create-a-group"></a>Ryhmän luominen

Tässä ohje aiheessa kerrotaan ryhmän luomisesta.

**Ryhmän luomis oikeudet**

Varmista, että sinulla on oikeus luoda uusi ryhmä. Yleiset järjestelmänvalvojat voivat poistaa ryhmän luomisen käytöstä Azure-portaalissa tai-paneelissa. Sinun on ehkä luotava uusi ryhmä puolestasi tai annettava sinulle tarvittavat käyttö oikeudet.

**Ryhmän luomisen käyttö oikeuksien hallinta**

1. Yleiset järjestelmänvalvojat voivat hallita ryhmän luomis oikeuksia (turvallisuussyistä) tai Office 365-ryhmiä, jotka on luotu Azure-portaalissa tai-ohjaus paneelissa valitsemalla "käyttäjät voivat luoda käyttö oikeus ryhmiä Azure Portals-sovelluksessa" tai "käyttäjät voivat luoda Office 365-ryhmiä Azure Portals"-asetukset **kaikkien ryhmien**  >  **Yleiset-kohdassa (asetukset)**.
2. Voit myös rajoittaa ryhmän luontia ja valita käyttäjä ryhmän, jos käytössä on Azure Active Directory P1 Premium-käyttö oikeus.

**Tervetuloa-ilmoituksen poistaminen käytöstä uusissa Office 365-ryhmän jäsenille**

Office 365-ryhmiin lisätyille käyttäjille lähetetyt tervetuloilmoitukset voidaan poistaa käytöstä määrittämällä Määritä **yksilöllinen Groupwelcomemessage** -asetukseksi false PowerShellin avulla. Lisä tietoja tästä asetuksesta on [täällä](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

