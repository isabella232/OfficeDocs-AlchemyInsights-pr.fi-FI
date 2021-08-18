---
title: 2491 Vuokraajan tai käyttäjän ohituskäytännön (Phish Delivered due to tenant or user override) sähköpostiviestien ilmoitus
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 90b078147bbb1e60cba0a2de6e49a862469f93aa
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316355"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Ilmoitus sähköpostiviesteihin Vuokraajan tai käyttäjän ohituksen vuoksi -phish Delivered due to tenant or user override -tekniikasta

Oletusilmoituskäytäntö nimeltä **Phish Toimitettu** vuokraajan tai käyttäjän ohituksen vuoksi on käytettävissä organisaatioissa, joissa on Microsoft Defender for Office 365 P1- ja P2-käyttöoikeudet. Jos sait tämän ilmoituksen, voit tutkia asian seuraavasti:

1. Siirry ilmoitusportaalin **Ilmoitukset-sivulle** valitsemalla **ilmoitusviestissä** Näytä Microsoft 365 Defender ilmoitus.

2. Valitse ilmoitus, jos haluat nähdä vaihtoehdon Näytä **viestiluettelo tai** **Näytä viestit Resurssienhallinnassa**. Kummallakin vaihtoehdolla voit tarkastella viestin tietoja, joihin sisältyy viestitunnus. Huomaa, että Threat Explorer -linkki suodattaa automaattisesti ilmoitukset, jotka vastaavat ilmoitusehtoja. Saatat joutua muokkaamaan päivämääräsuodatinta Threat Explorerissa.

Tietojen kalasteluviesti toimitettiin manuaalisesti määritetyn ohituksen vuoksi:

- Käyttäjän määrittämä sallittu lähettäjä tai toimialue.
- Sallittu lähettäjä tai toimialue, jonka järjestelmänvalvoja on määrittänyt roskapostin estokäytännön mukaisesti.
- Sallittu IP-osoite yhteyssuodatinkäytännön avulla.
- Postinkulkusääntö (kutsutaan myös siirtosäännöksi), joka on määritetty sallimaan viestit.

Jos viesti on mielestäsi merkitty virheellisesti [](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission) tietojen kalasteluksi, ilmoita viestistä Microsoftille järjestelmänvalvojan lähetyksen avulla.

Käyttäjät voivat lähettää [viestiesinäytteitä Microsoftille](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) Käyttämällä Ilmoita viestistä -apuohjelmaa Outlook Report Phishing -apuohjelmaa.
