---
title: Teams-hallintakeskus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: d504a26ee6532ec291eae797b1c81d86a05414b0
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354085"
---
# <a name="teams-admin-center"></a>Teams-hallintakeskus

Lisätietoja Teamsin hallinnasta [Teams-hallintakeskuksessa](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Jos et voi käyttää Teams-hallintakeskusta, varmista seuraavat asiat:

- Vahvista, että olet sallinut oikeat [Office 365:n IP-osoitteet ja URL-osoitteet](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) kaikissa eteisverkon laitteissa (kuten palomuuri) tai paikallisen laitteesi palomuurisäännöissä.
- Vahvista, että Teams-hallintaportaalissa käyttämäsi kirjautumistunnus vastaa [Microsoft 365 -hallintakeskuksessa](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) lueteltua käyttäjätunnusta.

Jos käyttäjiä ei näy Teams-hallintakeskuksessa, varmista seuraavat asiat:

- Oletko luonut käyttäjiä tai määrittänyt käyttöoikeuksia viimeksi kuluneiden 24 tunnin aikana? Varmista, että odotat vähintään 24 tuntia ennen tukipyynnön avaamista.
- Varmista, että olet määrittänyt oikeat käyttöoikeudet.
- Jos käytössäsi on paikallinen Active Directory, varmista, että [paikallisen Active Directoryn ProxyAddresses-kentän msRTCSIP-PrimaryUserAddress- tai SIP-osoitteen arvo on yksilöllinen ja että muoto vastaa](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip: Käyttäjän**käyttäjänimi** [Microsoft 365 -hallintakeskuksesta](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).
- Jos aiot pitää Skype for Business Serverin käyttöönoton ja käyttäjät ovat kotisi paikallisessa ja online-tilassa: noudata Skype for Business Serverin ohjauspaneelin **"Määritä yhdistelmä Teamsin ja Skype for Business Onlinen avulla"** -painiketta ja siirrä käyttäjät online-tilaan.
