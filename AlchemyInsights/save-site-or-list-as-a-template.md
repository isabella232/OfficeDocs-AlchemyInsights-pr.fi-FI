---
title: Sivuston tai luettelon tallentaminen mallina
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 31cb294be6b72be313cf63ed5ed2af0ef041dcf6efb7a7a2af4e1b6a9a149c43
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54109201"
---
# <a name="save-site-or-list-as-a-template"></a>Sivuston tai luettelon tallentaminen mallina

SharePoint sivustomallit ovat esimääritelmiä, jotka on suunniteltu tietyn liiketoimintatarpeen ympärille. Lisätietoja on kohdassa [Erityyppisten sivustojen luominen mallien SharePoint.](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)

Seuraavassa on joitakin yleisiä ongelmia/ratkaisuja, jotka liittyvät sivuston tai luettelon tallentamiseen mallina SharePoint Onlinessa.

**Tallenna sivusto/luettelomalli -painike ei ole käytettävissä tai puuttuu**. 

- Järjestelmänvalvojien on sallittava mukautettu komentosarja, jotta malliominaisuudet voidaan ottaa käyttöön. Yksityiskohtaiset ohjeet ovat esimerkeissä ja huomioissa [kohdassa Mukautetun komentosarjan salliminen tai estäminen.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)


- Tallenna sivusto malliksi -komentoa ei tueta, ja se voi aiheuttaa ongelmia sivustoissa, jotka käyttävät SharePoint Server -julkaisuinfrastruktuuria.


**Sivustomallia ei voi luoda tai se ei toimi oikein**

- Mallista saattaa puuttua [ominaisuus,](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) joka ei aktivoidu. Jos ominaisuus ei ole aktivoitavissa nykyisessä sivustokokoelmassa, et voi käyttää sivustomallia sivuston luomiseen.


- Tarkista, ettei missään luettelossa tai kirjastossa ole ylitetty [luettelonäkymän raja-arvoa](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59), joka on 5000 kohdetta, sillä se voi estää sivustomallin luomisen.


- Sivustossa voi olla käytössä liian monta resurssia, joten sivustomalli ylittää 50 megatavun (Mt) rajan.


- Tietoja näyttämisessä luettelosta, joka käyttää hakusaraketta, ilmeni ongelmia. Lisätietoja on kohdassa Mallin pohjalta luotu luettelo ei näytä oikean hakuluettelon tietoja [SharePoint Onlinessa.](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)


Lisätietoja yleisimpiä ongelmia ja ratkaisuja on kohdassa [Sivustomallien luominen ja käyttäminen.](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)

