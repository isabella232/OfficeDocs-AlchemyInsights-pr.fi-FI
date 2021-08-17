---
title: Sivuston luominen SharePoint Onlinessa
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057963"
---
# <a name="create-sharepoint-sites-using-templates"></a>Sivustojen SharePoint mallien avulla

Moderni viestintä tai ryhmäsivustot eivät tue mahdollisuutta tallentaa sivustoa mallina. Lisätietoja mallien käyttämisestä on kohdassa [Tallenna, lataa ja lataa palvelimeen SharePoint-sivusto mallina](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Seuraavassa on joitakin yleisiä ongelmia/ratkaisuja, jotka liittyvät sivuston tai luettelon tallentamiseen mallina SharePoint Onlinessa. 

**Tallenna sivusto tai luettelomalli -painike ei ole käytettävissä tai puuttuu**

Järjestelmänvalvojien on sallittava mukautettu komentosarja, jotta malliominaisuudet voidaan ottaa käyttöön. Yksityiskohtaiset ohjeet, esimerkit ja huomioon otettavia seikkoja ovat kohdassa 

- [Mukautetun komentosarjan salliminen tai estäminen](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Tallenna sivusto malliksi -komentoa ei tueta, ja se voi aiheuttaa ongelmia sivustoissa, jotka käyttävät SharePoint Server -julkaisuinfrastruktuuria.

**Sivustomallia ei voi luoda tai se ei toimi oikein**

Mallista saattaa puuttua [ominaisuus,](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) joka ei aktivoidu. Jos ominaisuus ei ole aktivoitavissa nykyisessä sivustokokoelmassa, et voi käyttää sivustomallia sivuston luomiseen.

- Tarkista, ettei missään luettelossa tai kirjastossa ole ylitetty [luettelonäkymän raja-arvoa](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59), joka on 5000 kohdetta, sillä se voi estää sivustomallin luomisen.

- Sivustossa voi olla käytössä liian monta resurssia, ja siksi sivustomalli ylittää 50 Mt:n rajan.


- Tietoja näyttämisessä luettelosta, joka käyttää hakusaraketta, ilmeni ongelmia. Lisätietoja on ohjeartikkelissa [Mallista luotu luettelo ei näytä oikean hakuluettelon tietoja SharePoint Onlinessa](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Lisätietoja yleisimpiä ongelmia ja ratkaisuja on kohdassa [Sivustomallien](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)luominen ja käyttäminen.



