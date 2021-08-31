---
title: Aktivointiongelma – Yhteyttä ei voida muodostaa juuri nyt
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
- "3408"
- "9001423"
ms.openlocfilehash: 0ab831696736352bf9de84f43c96bb8f7238d8eb
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744592"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Viestin Microsoft 365 yhteyttä ei voi muodostaa juuri nyt -sanoman asentaminen

Huomautus: Jos käytät Windows:n vanhempaa versiota (esimerkiksi Windows 7 SP1- tai Windows Server 2008 R2 [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) -versiota), ota TLS 1.2 käyttöön oletusarvoisesti helpon korjauksen avulla. Lisätietoja on päivityksessä [TLS 1.1: n ja TLS 1.2:n ottaminen](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)käyttöön WinHTTP in Windows :n oletusarvoisen suojatun protokollan avulla.

Jos näyttöön tulee tämä sanoma, kokeile seuraavaa:

1. Tarkista palomuurin, virustentorjuntaohjelman ja välityspalvelimen asetukset ja varmista, että ne eivät estä Microsoft 365 internet-yhteyttä. Katso [Microsoftin URL-osoitteet ja IP-osoitealueet.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Siirry Käynnistä **Suorita**  >  **-valikkoon** ja kirjoita **services.msc.** Varmista, että seuraavat palvelut ovat käynnissä:
    - Verkkoon yhdistetyt laitteet – automaattinen määritys
    - Verkkoluettelopalvelu
    - Verkkosijainnin tietoisuus
    - Windows Tapahtumaloki

Jos jokin näistä palveluista ei ole käynnissä, yritä käynnistää se. Jos palvelun avaamisessa ilmenee ongelmia, suorita seuraava komento avaamalla komentokehote, jossa on järjestelmänvalvojan oikeudet:

**sfc /scannow**

Kun tämä komento on valmis, käynnistä tietokone uudelleen.

Lisätietoja on kohdassa ["Yhteyttä tiliisi ei valitettavasti voi muodostaa. Yritä myöhemmin uudelleen"-virhe aktivoitaessa Office Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)