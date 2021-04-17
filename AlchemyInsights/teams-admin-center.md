---
title: Teams-hallintakeskus
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826376"
---
# <a name="teams-admin-center"></a>Teams-hallintakeskus

Lisätietoja Teamsin hallinnasta [Teams-hallintakeskuksessa](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Jos et voi käyttää Teams-hallintakeskusta, varmista seuraavat asiat:

- Vahvista, että olet sallinut oikeat [Office 365:n IP-osoitteet ja URL-osoitteet](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) kaikissa eteisverkon laitteissa (kuten palomuuri) tai paikallisen laitteesi palomuurisäännöissä.
- Vahvista, että Teams-hallintaportaalissa käyttämäsi kirjautumistunnus vastaa [Microsoft 365 -hallintakeskuksessa](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) lueteltua käyttäjätunnusta.

Jos käyttäjiä ei näy Teams-hallintakeskuksessa, varmista seuraavat asiat:

- Oletko luonut käyttäjiä tai määrittänyt käyttöoikeuksia viimeksi kuluneiden 24 tunnin aikana? Varmista, että odotat vähintään 24 tuntia ennen tukipyynnön avaamista.
- Varmista, että olet määrittänyt oikeat käyttöoikeudet.
- Jos käytössäsi on paikallinen Active Directory, varmista, että [paikallisen Active Directoryn ProxyAddresses-kentän msRTCSIP-PrimaryUserAddress-](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) tai SIP-osoite on yksilöllinen ja muoto vastaa muotoa **sip:** Käyttäjän käyttäjänimi [Microsoft 365 -hallintakeskuksesta.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)
- Jos aiot pitää Skype for Business Serverin käyttöönoton ja määrittää käyttäjät kotikäyttöön paikallisesti ja verkossa: seuraa Skype for Business Serverin Ohjauspaneelissa **olevaa "Set up hybrid with Teams and Skype for Business Online"** (Teamsin ja Skype for Business Onlinen yhdistelmäympäristön määrittäminen) -ohjetta ja siirrä käyttäjiä verkossa.
