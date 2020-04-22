---
title: Office-sovellusten korjaaminen Valitettavasti meillä on tilapäispalvelinongelmien sanoma
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764114"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Office-sovellusten korjaaminen "Anteeksi, meillä on tilapäisiä palvelinongelmia" -sanoma

Jos saat tämän sanoman, kokeile seuraavaa:

1. Tarkista palomuurin, virustentorjuntaohjelmiston ja välityspalvelimen asetukset ja varmista, että ne eivät estä Office-sovellusten Internet-yhteyttä. Katso [URL-osoitteet ja IP-osoitealueet](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Siirry **Käynnistä-kohtaan** > **Run**ja kirjoita **services.msc**. Varmista, että seuraavat palvelut ovat käynnissä:
    - Verkkoon liitettyjen laitteiden automaattinen asennus
    - Verkkoluettelopalvelu
    - Verkon sijaintitietoisuus
    - Windowsin tapahtumaloki

Jos jokin näistä palveluista ei ole käynnissä, yritä käynnistää se. Jos palvelun käynnistämisessä on ongelmia, suorita seuraava komento avaamalla komentorivi, jolla on laajennetut käyttöoikeudet:

**Kävi koulua sfc /scannow**

Kun tämä komento on valmis, käynnistä tietokone uudelleen.

Lisätietoja on kohdassa ["Valitettavasti emme voi muodostaa yhteyttä tiliisi. Yritä myöhemmin uudelleen" -virhe aktivoitaessa.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)