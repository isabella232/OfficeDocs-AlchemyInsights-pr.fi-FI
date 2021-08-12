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
ms.openlocfilehash: 7922a2c5306f9d16856502b5e57e585cb90f2f7c9abaad0366f72ed46de786d5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957097"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a>Ehdotuksia "Ei käyttöommeniton tuote" -virheiden ratkaisemiseen

Voit ratkaista Lisensoimaton tuote -virheilmoituksia seuraavasti:

- Tarkista, onko tilauksesi tila vanhentunut.
- Varmista, että sinulla on tilaus, joka sallii asiakkaan käyttöoikeudet, kuten Microsoft 365 -sovellukset yrityksille tai Business Premium, ja varmista, että käyttäjälle [on määritetty käyttöoikeus.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) 
- Varmista, että käyttäjä kirjautuu Office samalla tilillä, jolla käyttöoikeus on määritetty.
- Tarkista [Palvelun kunto -sivulta,](https://docs.microsoft.com/office365/enterprise/view-service-health) onko palvelussa tunnettuja ongelmia.
- Tarkista palomuurin, virustentorjuntaohjelman ja välityspalvelimen asetukset ja varmista, että ne Microsoft 365 internet-yhteyttä. Katso [URL-osoitteet ja IP-osoitealueet.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

Voit myös kokeilla seuraavia vianmääritystoimia: 

- Avaa Office-sovellus ja [kirjaudu ulos](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) olemassa olevista käyttäjätileistä. [Poista](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) [ja määritä käyttöoikeus](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office uudelleen ja [kirjaudu](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) sitten Office käyttäjätilillä.
- Suorita [aktivoinnin vianmääritys.](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Palauta Officen aktivoinnin tila](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state). 
- [Suorita online-korjaus Office.](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b)

Lisätietoja vianmäärityksestä on seuraavissa artikkeleissa: 

- [Ei käyttöoikeutta -virheet ja aktivointivirheet Officessa](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [”Emme voi muodostaa yhteyttä tiliisi. Yritä myöhemmin uudelleen" -virhe Officen aktivoinnin yhteydessä](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)