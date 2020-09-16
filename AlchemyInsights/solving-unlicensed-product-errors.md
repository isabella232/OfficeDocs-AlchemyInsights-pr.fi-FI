---
title: Lisensoimattomien tuote virheiden ratkaiseminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: bd2e8cb204edd7135fc34ef0d42ac8259434d37d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737950"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Ehdotuksia "käyttöoikeudettoman tuotteen" virheiden ratkaisemiseksi

Jos haluat ratkaista Käyttöoikeudetonta tuotetta koskevia virheitä, kokeile seuraavaa:

- Tarkista, onko tilauksesi tila vanhentunut.
- Varmista, että sinulla on tilaus, joka sallii asiakas käyttö oikeudet, kuten Microsoft 365-sovellukset Business-tai Business Premium-sovelluksessa, ja varmista, [että käyttäjälle on määritetty käyttö oikeus](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). 
- Varmista, että käyttäjä on kirjautunut Officeen samalla tilillä, jolle käyttö oikeus on määritetty.
- Tarkista [palvelun kunto-sivulla](https://docs.microsoft.com/office365/enterprise/view-service-health) , onko palvelussa tiedossa ongelmia.
- Tarkista palo muurin, virustentorjuntaohjelman ja välitys palvelimen asetukset ja varmista, että ne eivät estä Microsoft 365-sovelluksia, jotka käyttävät Internetiä. Katso [URL-osoitteet ja IP-osoite alueet](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Voit myös kokeilla seuraavia vian määritys toimia: 

- Avaa Office-sovellus ja [Kirjaudu ulos](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) olemassa olevista käyttäjä tileistäsi. [Poista](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) Office-käyttö oikeus ja [Määritä se uudelleen](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ja [Kirjaudu sitten sisään Officeen](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) haavoittuvuuden sisältävän käyttäjä tilin avulla.
- Suorita [Akti voinnin vian määritys](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Palauta Officen aktivoinnin tila](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Suorita Officen online-korjaus](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Lisätietoja vianmäärityksestä on seuraavissa artikkeleissa: 

- [Ei käyttöoikeutta -virheet ja aktivointivirheet Officessa](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [”Emme voi muodostaa yhteyttä tiliisi. Yritä myöhemmin uudelleen" -virhe Officen aktivoinnin yhteydessä](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)