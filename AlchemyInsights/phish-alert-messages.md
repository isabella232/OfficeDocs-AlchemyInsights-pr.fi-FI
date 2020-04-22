---
title: 2491 Ilmoita Phish Delivered -palvelun sähköpostiviestit vuokralaisen tai käyttäjän ohituskäytännön vuoksi
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758921"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Ilmoita Phish Delivered -palvelun sähköpostiviestit vuokraajan tai käyttäjän ohituksen vuoksi -käytännöstä

Oletushälytyskäytäntö nimeltä "Phish Toimitettu vuokraajan tai käyttäjän ohituksen vuoksi" on otettu käyttöön vuokraajille, joilla on Office 365 ATP P1- ja P2-käyttöoikeudet. Jos sait tämän ilmoituksen, voit tutkia seuraavia ohjeita:

1. Siirry Suojaus-& yhteensopivuuskeskuksen **Hälytykset-sivulle** valitsemalla **ilmoitusviestin.**

2. Valitse ilmoitus, jos haluat nähdä vaihtoehdon **Näytä viestiluettelo** tai **Näytä viestit Resurssienhallinnassa**. Molemmat näistä vaihtoehdoista vievät viestin tiedot, jotka sisältävät viestin tunnuksen. Huomaa, että Threat Explorer -linkki suodattaa automaattisesti sanomaehtoja vastaavat viestit. Päivämääräsuodatinta on ehkä muutettava Threat Explorerissa.

Tietojenkalasteluviesti toimitettiin manuaalisesti määritetyn ohituksen vuoksi:

- Käyttäjän määrittämä sallittu lähettäjä tai toimialue.

- Järjestelmänvalvojan roskapostin vastaisessa käytännössä määrittämä sallittu lähettäjä tai toimialue.

- Yhteyssuodatinkäytännön sallittu IP-osoite.

- Postin kulkusääntö (jota kutsutaan myös siirtosäännöksi), joka on määritetty sallimaan viestit.

Jos uskot, että viesti on virheellisesti merkitty phish-merkinnäksi, lähetä viestiesimerkit Microsoftille [Outlookin raporttiviesti -apuohjelman](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) avulla.
