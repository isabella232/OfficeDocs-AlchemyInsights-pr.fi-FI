---
title: Kirjautuminen ei onnistu Teamsiin virheen autologon.microsoftazuread-sso.com:443 vuoksi
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931901"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>Kirjautuminen ei onnistu Teamsiin virheen autologon.microsoftazuread-sso dot com:443 vuoksi

Jos saumaton kertakirjautuminen on otettu käyttöön O365-todennuksena, intranet-sivustoille on ehkä lisättävä URL-osoite ”autologon.microsoftazuread-sso.com”.  Jos se on aiemmin lisätty luotettaville sivustoille ja saumaton kertakirjautuminen on käytössä, se on poistettava luotettavista sivustoista.

Tarkista [saumattoman kertakirjautumisen vianmäärityksen tarkistusluettelo](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).

Voit lisätä URL-osoitteen intranet-sivustojen luetteloon seuraavien ohjeiden mukaisesti:

1. Avaa Internet Explorer napsauttamalla **Käynnistä**-painiketta. Kirjoita hakukenttään Internet Explorer ja napsauta sitten tulosluettelosta **Internet Explorer**.
2. Napsauta **Työkalut** ja napsauta sitten **Internet-asetukset**.
3. Napsauta **Suojaus**-välilehteä.
4. Napsauta nyt **Paikalliset intranet-sivustot** ja napsauta sitten **Sivustot**-painiketta ja sitten **Lisäasetukset**-painiketta.
5. Kirjoita verkkosivuston URL-osoite ja napsauta **Lisää**.
6. Kun olet valmis, napsauta **Sulje**.

Katso lisätietoja artikkelista [O365:n saumattoman kertakirjautumisen käyttöönotto-ohjeet](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (sisältää käytäntöpohjaisen prosessin URL-osoitteen lisäämiseksi intranet-sivustoille vaiheessa 3).
