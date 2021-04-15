---
title: Ei käyttöomme -virheiden ratkaiseminen
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
- "3412"
- "9001428"
ms.openlocfilehash: eebfb7cea7ae97921bf3c3667818400a17b5e52e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786846"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Ehdotuksia "Ei käyttöommeniton tuote" -virheiden ratkaisemiseen

Voit ratkaista Lisensoimaton tuote -virheilmoituksia seuraavasti:

- Tarkista, onko tilauksesi tila vanhentunut.
- Varmista, että sinulla on tilaus, joka sallii asiakkaan käyttöoikeudet, kuten Microsoft 365 Apps for Business tai Business Premium, ja varmista, että käyttäjälle [on määritetty käyttöoikeus.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) 
- Varmista, että käyttäjä kirjautuu Officeen samalla tilillä, jolla käyttöoikeus on määritetty.
- Tarkista [Palvelun kunto -sivulta,](https://docs.microsoft.com/office365/enterprise/view-service-health) onko palvelussa tunnettuja ongelmia.
- Tarkista palomuurin, virustentorjuntaohjelman ja välityspalvelimen asetukset ja varmista, että ne eivät estä Microsoft 365 -sovellusten Internet-yhteyttä. Katso [URL-osoitteet ja IP-osoitealueet.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

Voit myös kokeilla seuraavia vianmääritystoimia: 

- Avaa Office-sovellus ja [kirjaudu ulos](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) olemassa olevista käyttäjätileistä. [Poista](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) ja [määritä Office-käyttöoikeus](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) uudelleen ja kirjaudu sitten [Sisään Officeen](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) käyttäen käyttäjätiliä, jota ongelma koskee.
- Suorita [aktivoinnin vianmääritys.](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Palauta Officen aktivoinnin tila](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Suorita Officen Online-korjaus.](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)

Lisätietoja vianmäärityksestä on seuraavissa artikkeleissa: 

- [Ei käyttöoikeutta -virheet ja aktivointivirheet Officessa](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [”Emme voi muodostaa yhteyttä tiliisi. Yritä myöhemmin uudelleen" -virhe Officen aktivoinnin yhteydessä](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)