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
ms.openlocfilehash: 9771a3244c5507312d43156525095fb9eaf7fa20
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812569"
---
# <a name="unable-to-activate-office"></a>Officen aktivointi epäonnistui

- Tarkista, onko tilauksesi vanhentunut.
- Varmista, että käyttöoikeutesi sallii asiakaskäyttöoikeudet, kuten Office 365 Businessin tai Business Premiumin, ja että [käyttäjälle on määritetty käyttöoikeus](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).
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