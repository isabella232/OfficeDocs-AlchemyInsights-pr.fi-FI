---
title: Officen aktivointi epäonnistui
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
- "2000023"
- "3509"
ms.openlocfilehash: 9a33b7880aff6016ef6df88960d6f59ac9dd50382c7e99d72ca36bc3c9f344ea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928366"
---
# <a name="unable-to-activate-office"></a>Officen aktivointi epäonnistui

**Huomautus:** Jos käytät vanhempaa Windows (esimerkiksi Windows 7), varmista, että TLS 1.2 on käytössä oletusversiona. Lisätietoja on päivityksessä [TLS 1.1: n ja TLS 1.2:n käyttöönottamiseksi WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392):n oletusarvoina suojattuina protokollina.

- Tarkista, onko tilauksesi vanhentunut.
- Varmista, että käyttöoikeutesi sallii asiakaskäyttöoikeudet, kuten Office 365 Businessin tai Business Premiumin, ja että [käyttäjälle on määritetty käyttöoikeus](/microsoft-365/admin/manage/assign-licenses-to-users).
- Varmista, että käyttäjä kirjautuu Officeen tilillä, jolle on määritetty käyttöoikeus.
- Tarkista [Office 365:n palvelun kunto -sivulla](/office365/enterprise/view-service-health), onko palvelussa tunnettuja ongelmia.
- Tarkista palomuurin, virustorjuntaohjelmiston ja välityspalvelimen asetukset ja varmista, etteivät ne estä Microsoft 365 -sovellusten yhteyttä Internetiin. Lisätietoja on artikkelissa [Office 365:n URL-osoitteet ja IP-osoitealueet](/office365/enterprise/urls-and-ip-address-ranges "Office 365:n URL-osoitteet ja IP-osoitealueet").

**Vihje** Voimme diagnosoida ja korjata useita Windows-tietokoneiden Officen yleisiä sisäänkirjautumisongelmia puolestasi automaattisesti. Jos haluat käyttää automaattista työkaluamme, lataa ja suorita **[Microsoftin tuki- ja palautusavustaja](https://aka.ms/SaRA-OfficeSignInScenario)**.

Tee vianmääritys seuraavasti:

- Avaa Office-sovellus ja [kirjaudu ulos](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) olemassa olevilta käyttäjätileiltä. [Poista](/microsoft-365/admin/manage/remove-licenses-from-users) ja [määritä uudelleen](/microsoft-365/admin/manage/assign-licenses-to-users) Office-käyttöoikeus ja [kirjaudu sitten Officeen](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) käyttämällä kyseistä käyttäjätiliä.
- [Aktivoinnin vianmääritysohjelman](https://aka.ms/SARA-OfficeActivation-Alchemy) suorittaminen
- [Officen aktivoinnin tilan palauttaminen](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Officen aktivoinnin tilan palauttaminen")
- [Officen online-korjauksen suorittaminen](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Lisätietoja vianmäärityksestä on seuraavissa artikkeleissa:  

- [Ei käyttöoikeutta -virheet ja aktivointivirheet Officessa](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [”Emme voi muodostaa yhteyttä tiliisi. Yritä myöhemmin uudelleen" -virhe Officen aktivoinnin yhteydessä](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)