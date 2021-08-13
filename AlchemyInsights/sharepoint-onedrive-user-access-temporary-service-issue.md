---
title: Suorituskykyongelmat SharePoint tai OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 08bdc2527147279063e3f66a1767203e5ccdc1dd4fd8b871f2800d3f71b9a233
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093725"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint tai OneDrive, Useiden käyttäjien ei voi käyttää tai olla käytettävissä

Jos OneDrive tai SharePoint ei ole useiden käyttäjien käytettävissä, joilla oli aiemmin käyttöoikeus, palvelu voi olla tilapäinen. [Tarkista palvelun kunto -koontinäyttö](https://portal.office.com/adminportal/home#/servicehealth).

**Käyttäjän lisääminen ja käyttöoikeuden lisääminen**

Varmista, että [määrität käyttöoikeudet käyttäjille Microsoft 365 for Businessissa.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)


**Käyttöoikeuksien määrittäminen**

Jos käyttäjälle on määritetty SharePoint-käyttöoikeus ja hän saa edelleen käyttö estetty -viestin, varmista, että hänelle on määritetty [asianmukainen](https://docs.microsoft.com/sharepoint/understanding-permission-levels) käyttöoikeustaso.

**Käyttöoikeuspyyntötoiminnon käyttäminen**

[Käyttöoikeuspyyntötoiminnon avulla](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) käyttäjät voivat pyytää käyttöoikeuksia sisältöön, jota heillä ei tällä hetkellä ole.

**Salli mukautettu komentosarja voi aiheuttaa käyttö estetty -ongelmia**

Joissakin tilanteissa Allow *custom script (Salli* mukautettu komentosarja) -ominaisuus saattaa esittää käyttö estetty -toiminnon. Jos haluat luettelon ominaisuuksista, joihin tämä vaikuttaa, ota huomioon suojausta ja mahdollisuus poistaa ominaisuus käytöstä. Siirry [mukautetun komentosarjan salliminen tai estäminen -lta.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

