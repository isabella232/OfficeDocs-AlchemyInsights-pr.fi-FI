---
title: 'Sähköpostin lähettäminen tai vastaanottaminen Office 365:lle tai Office 365:stä ei onnistu TLS 1.0: n ja TLS 1.1:n käytöstä poistamisen vuoksi'
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745019"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Sähköpostin lähettäminen tai vastaanottaminen Office 365:lle tai Office 365:stä ei onnistu TLS 1.0: n ja TLS 1.1:n käytöstä poistamisen vuoksi

Kuten viestikeskuksen mc229914-jälkeinen viesti on vahvistanut, TLS 1.0- ja TLS 1.1 -poisto aloitettiin Exchange Onlinen postinkulkupäätepisteiden käytön. Pian Office 365 ei enää hyväksy TLS 1.0- ja TLS 1.1 -sähköpostiyhteyksiä ulkoisista lähteistä. Exchange Online ei myöskään koskaan käytä TLS 1.0: ta tai 1.1 lähtevän sähköpostin lähettämiseen. Jos kohtaat ongelmia TLS 1.0:n tai 1.1:n käytöstä poistamisen vuoksi, saatat kohdata yhden seuraavista virheistä:

- Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'
- Virhe paikallisen palvelimen Jonon katseluohjelmassa, joka lähettää sähköpostia Officer 365:lle– '421 4.4.2 Yhteys katkesi SocketErrorin vuoksi'
- Virhe Lähetä [yhdistinprotokolla -lokissa](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) palvelimessa, joka lähettää sähköpostia Office 365:lle– TLS-neuvottelu epäonnistui virheen SocketError kanssa
- Virhe yhdistinprotokollan lähetys- tai vastaanottolokissa – '451 5.7.3 StartTLS-komento on ensin annettava'

Jos ilmenee jokin yllä mainituista virheistä, varmista, että sähköpostia lähettävällä tai vastaanottavalla palvelimella on TLS 1.2 käytössä, tarkistamalla seuraavat rekisteriavaimet:

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Asiakas] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001**

Jos teet muutoksia yllä mainittuihin rekisteriavaimiin TLS 1.2:n käyttöönottoon, käynnistä palvelin uudelleen, jotta muutokset tulevat voimaan. Varmista myös, että olet asentanut uusimmat Windows- ja Exchange-päivitykset.

Lisätietoja on seuraavissa artikkeleissa:

- [Exchange Serverin TLS-ohjeet, osa 1: Valmistautuminen TLS 1.2:ta varten – Microsoft Tech Community -yhteisö](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Serverin TLS-ohjeet, osa 2: TLS 1.2:n ottaminen käyttöön ja asiakkaiden tunnistaminen, jotka eivät käytä sitä - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Sähköpostiskenaarioiden ymmärtäminen, jos TLS-versioita ei voi hyväksyä Exchange Onlinen avulla – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
