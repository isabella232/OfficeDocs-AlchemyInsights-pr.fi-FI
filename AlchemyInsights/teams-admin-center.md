---
title: Teams-hallintakeskus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670361"
---
# <a name="teams-admin-center"></a>Teams-hallintakeskus

Lisätietoja Teamsin hallinnasta [Teams-hallintakeskuksessa](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Jos et voi käyttää Teams-hallintakeskusta, varmista seuraavat asiat:

- Vahvista, että olet sallinut oikeat [Office 365:n IP-osoitteet ja URL-osoitteet](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) kaikissa eteisverkon laitteissa (kuten palomuuri) tai paikallisen laitteesi palomuurisäännöissä.
- Vahvista, että Teams-hallintaportaalissa käyttämäsi kirjautumistunnus vastaa [Microsoft 365 -hallintakeskuksessa](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) lueteltua käyttäjätunnusta.

Jos käyttäjiä ei näy Teams-hallintakeskuksessa, varmista seuraavat asiat:

- Oletko luonut käyttäjiä tai määrittänyt käyttöoikeuksia viimeksi kuluneiden 24 tunnin aikana? Varmista, että odotat vähintään 24 tuntia ennen tukipyynnön avaamista.
- Varmista, että olet määrittänyt oikeat käyttöoikeudet.
- Jos käytössäsi on paikallinen Active Directory-hakemisto, varmista, että [paikallisen Active Directoryn ProxyAddresses-kentässä oleva Msrtcssip-Primaruseraddress-tai SIP-osoitteen arvo on yksilöllinen ja että muoto vastaa](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) SIP: käyttäjän**käyttäjä nimeä** [Microsoft 365-hallinta keskuksesta](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Jos haluat säilyttää Skype for Business-palvelimen käyttöönoton ja pitää käyttäjät paikallisessa verkossa ja online-tilassa: Seuraa **"Määritä yhdistelmä käyttö teamsin ja Skype for Business Onlinen avulla"** Skype for Business Serverin ohjaus paneelissa ja siirrä käyttäjät online-tilassa.
