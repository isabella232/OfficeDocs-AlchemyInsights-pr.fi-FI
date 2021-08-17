---
title: 'Sähköpostin lähettäminen tai vastaanottaminen Office 365 TLS 1.0: n ja TLS 1.1:n käytöstä poistamisen vuoksi ei onnistu'
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
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054903"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Sähköpostin lähettäminen tai vastaanottaminen Office 365 TLS 1.0: n ja TLS 1.1:n käytöstä poistamisen vuoksi ei onnistu

Kuten viestikeskuksen MC229914-julkaisussa on vahvistettu, TLS 1.0: n ja TLS 1.1:n poisto alkoi ottaa Exchange Online postinkulkupäätepisteille. Pian Office 365 enää hyväksy TLS 1.0- ja TLS 1.1 -sähköpostiyhteyksiä ulkoisista lähteistä. Lisäksi Exchange Online ei koskaan käytä TLS 1.0: aa tai 1.1:tä lähtevän sähköpostin lähettämiseen. Jos kohtaat ongelmia TLS 1.0: n tai 1.1:n käytöstä poistamisen vuoksi, saatat kohdata yhden seuraavista virheistä:

- Lähettäjän NDR-virhe palautuu – '421 4.4.2 Yhteys katkesi SocketErrorin vuoksi'
- Virhe paikallisen palvelimen Jonon katseluohjelmassa, joka lähettää sähköpostia Officer 365:lle - '421 4.4.2 Yhteys katkesi SocketErrorin vuoksi'
- Virhe Lähetä [yhdistinprotokolla -lokissa](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) palvelimeen, joka lähettää sähköpostia Office 365- TLS-neuvottelu epäonnistui virheen SocketError kanssa
- Virhe Lähetä tai vastaanota -yhdistimen protokollalokissa – '451 5.7.3 On ensin tehtävä STARTTLS-komento"

Jos yllä mainitut virheet ilmenee, varmista, että sähköpostia lähettävällä tai vastaanottavilla palvelimella on TLS 1.2 käytössä tarkistamalla seuraavat rekisteriavaimet-

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Asiakas] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001**

Jos teet muutoksia yllä mainittuihin rekisteriavaimiin TLS 1.2:n käyttöönottoon, käynnistä palvelin uudelleen, jotta muutokset tulevat voimaan. Varmista myös, että olet asentanut uusimmat Windows ja Exchange päivitykset.

Lisätietoja on seuraavissa artikkeleissa:

- [Exchange Server TLS-ohjeet, osa 1: Valmistautuminen TLS 1.2 :tä varten – Microsoft Tech Community -yhteisö](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server TLS-ohjeet Osa 2: TLS 1.2:n ottaminen käyttöön ja Asiakkaiden tunnistaminen, jotka eivät käytä sitä - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Sähköpostiskenaarioiden ymmärtäminen, jos TLS-versioita ei voi hyväksyä Exchange Online - Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
