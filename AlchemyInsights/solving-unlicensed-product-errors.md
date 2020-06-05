---
title: Lisensoimattomien tuotevirheiden ratkaiseminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3412"
- "9001428"
ms.openlocfilehash: 89d0e589329d40f17c36baa54868154be0f5b887
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582736"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Ehdotuksia luvattoman tuotteen virheiden ratkaisemiseksi

Voit ratkaista "Lisensoimaton tuote" -virheitä seuraavasti:

- Tarkista, onko tilauksesi tila vanhentunut.
- Varmista, että sinulla on tilaus, joka sallii asiakaskäyttöoikeudet, kuten Microsoft 365 Apps for Business tai Business Premium, ja [varmista, että käyttäjälle on määritetty käyttöoikeus.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) 
- Varmista, että käyttäjä on kirjautuu Officeen samalla tilillä, jolle on määritetty käyttöoikeus.
- Tarkista [Palvelun kunto -sivulta,](https://docs.microsoft.com/office365/enterprise/view-service-health) onko palvelussa tunnettuja ongelmia.
- Tarkista palomuurin, virustentorjuntaohjelmiston ja välityspalvelimen asetukset ja varmista, että ne eivät estä Microsoft 365 -sovellusten Internet-käyttöä. Katso [URL-osoitteet ja IP-osoitealueet](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

Voit myös kokeilla seuraavia vianmääritystoimia: 

- Avaa Office-sovellus ja [kirjaudu ulos](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) olemassa olevista käyttäjätileistä. [Poista](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) [Office-käyttöoikeus](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) ja määritä se uudelleen ja kirjaudu sitten [Officeen](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) käyttämällä kyseistä käyttäjätiliä.
- Suorita [aktivoinnin vianmääritys](https://aka.ms/SARA-OfficeActivation-Alchemy).
- [Palauta Officen aktivoinnin tila](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Officen online-korjauksen suorittaminen](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).

Lisätietoja vianmäärityksestä on seuraavissa artikkeleissa: 

- [Ei käyttöoikeutta -virheet ja aktivointivirheet Officessa](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [”Emme voi muodostaa yhteyttä tiliisi. Yritä myöhemmin uudelleen" -virhe Officen aktivoinnin yhteydessä](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)