---
title: Suorituskyky ongelmat-SharePoint tai OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771241"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePointin tai OneDriven hidas, saavuttamattomissa tai poissa käytöstä useille käyttäjille

Jos OneDrive-tai SharePoint-sivusto ei ole käytettävissä useille käyttäjille, joilla on aiemmin ollut käyttö oikeus, kyseessä saattaa olla väliaikainen palvelu ongelma. [Tarkista palvelun kunnon koonti näyttö](https://portal.office.com/adminportal/home#/servicehealth).

**Käyttäjän lisääminen ja käyttö oikeuksien määrittäminen**

Varmista, että määrität [käyttäjille käyttö oikeudet Microsoft 365 for Businessissa](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).


**Käyttö oikeuksien määrittäminen**

Jos käyttäjälle on määritetty SharePoint-käyttö oikeus ja saat edelleen käyttö estetty-viestin, varmista, että hänelle on määritetty [tarvittava käyttö oikeus taso](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .

**Käyttö oikeus pyyntö toiminnon käyttäminen**

[Käyttö oikeus pyyntö-toiminnon](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) avulla käyttäjät voivat pyytää käyttö oikeutta sisältöön, jota heillä ei tällä hetkellä ole oikeus nähdä.

**Salli mukautettu komento sarja voi aiheuttaa käyttö estetty-ongelmia**

On olemassa tiettyjä tilanteita, joissa *Salli mukautettu komento sarja* -ominaisuus voi esittää käyttö estetty-toiminnon. Luettelo ominaisuuksista, joihin ongelma vaikuttaa, tieto turvaan liittyviä seikkoja ja mahdollisuus poistaa ominaisuus käytöstä. Tutustu [Salli-tai estä mukautettua komento sarjaa](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).

