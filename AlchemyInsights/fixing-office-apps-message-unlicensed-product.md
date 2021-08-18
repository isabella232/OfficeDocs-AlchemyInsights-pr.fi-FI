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
ms.openlocfilehash: a057aaa2ddf8885b96c0fe0d5fa87d3a1b191af9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327843"
---
# <a name="unable-to-activate-office"></a>Officen aktivointi epäonnistui

**Huomautus:** Jos käytät vanhempaa Windows -versiota (esimerkiksi Windows 7), varmista, että TLS 1.2 on käytössä oletusarvoisesti. Lisätietoja on päivityksessä [TLS 1.1: n ja TLS 1.2:n](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)ottaminen käyttöön WinHTTP in Windows :n oletusarvoisen suojatun protokollan avulla.

- Tarkista, onko tilauksesi vanhentunut.
- Varmista, että käyttöoikeutesi sallii asiakaskäyttöoikeudet, kuten Office 365 Businessin tai Business Premiumin, ja että [käyttäjälle on määritetty käyttöoikeus](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users).
- Varmista, että käyttäjä kirjautuu Officeen tilillä, jolle on määritetty käyttöoikeus.
- Tarkista [Office 365:n palvelun kunto -sivulla](https://docs.microsoft.com/office365/enterprise/view-service-health), onko palvelussa tunnettuja ongelmia.
- Tarkista palomuurin, virustorjuntaohjelmiston ja välityspalvelimen asetukset ja varmista, etteivät ne estä Microsoft 365 -sovellusten yhteyttä Internetiin. Lisätietoja on artikkelissa [Office 365:n URL-osoitteet ja IP-osoitealueet](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365:n URL-osoitteet ja IP-osoitealueet").

**Vihje** Voimme diagnosoida ja korjata useita Windows-tietokoneiden Officen yleisiä sisäänkirjautumisongelmia puolestasi automaattisesti. Jos haluat käyttää automaattista työkaluamme, lataa ja suorita **[Microsoftin tuki- ja palautusavustaja](https://aka.ms/SaRA-OfficeSignInScenario)**.

Tee vianmääritys seuraavasti:

- Avaa Office-sovellus ja [kirjaudu ulos](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) olemassa olevilta käyttäjätileiltä. [Poista](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) ja [määritä uudelleen](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office-käyttöoikeus ja [kirjaudu sitten Officeen](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) käyttämällä kyseistä käyttäjätiliä.
- [Aktivoinnin vianmääritysohjelman](https://aka.ms/SARA-OfficeActivation-Alchemy) suorittaminen
- [Officen aktivoinnin tilan palauttaminen](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Officen aktivoinnin tilan palauttaminen")
- [Officen online-korjauksen suorittaminen](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Lisätietoja vianmäärityksestä on seuraavissa artikkeleissa:  

- [Ei käyttöoikeutta -virheet ja aktivointivirheet Officessa](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [”Emme voi muodostaa yhteyttä tiliisi. Yritä myöhemmin uudelleen" -virhe Officen aktivoinnin yhteydessä](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)