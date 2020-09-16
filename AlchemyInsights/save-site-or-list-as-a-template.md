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
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727528"
---
# <a name="save-site-or-list-as-a-template"></a>Sivuston tai luettelon tallentaminen mallina

SharePoint-Sivustomallit ovat valmiita määritelmiä, jotka on suunniteltu tietyn yritys tarpeen ympärille. Lisä tietoja on kohdassa [mallien käyttäminen erilaisten SharePoint-sivustotyyppien luomiseen](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Seuraavassa on joitakin yleisiä ongelmia tai ratkaisuja, jotka liittyvät sivuston tai luettelon tallentamiseen SharePoint Onlinen mallina.

**Tallenna sivuston/luettelon malli-painike ei ole käytettävissä tai se puuttuu**. 

- Järjestelmänvalvojien on sallittava malli ominaisuuksien käyttöönotto mukautetulla komento sarjalla. Yksityiskohtaisia ohjeita, esimerkkejä ja Huomioitavaa on artikkelissa [mukautetun komento sarjan salliminen tai estäminen](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Tallenna sivusto mallina-komento ei ole käytettävissä, ja se voi aiheuttaa ongelmia SharePoint Serverin Julkaisuinfrastruktuuria käyttävien sivustojen kanssa.


**Sivustomallia ei voi luoda tai se ei toimi oikein**

- Mallista saattaa puuttua [ominaisuus](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , eikä se aktivoidu. Jos ominaisuus ei ole käytettävissä nykyisessä sivustokokoelmassa, sivustomallia ei voi käyttää sivuston luomiseen.


- Tarkista, ylittävätkö luettelot tai kirjastot 5000-kohteiden [luettelo näkymän raja-arvon](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) , sillä tämä voi estää sivustomallin luomisen.


- Sivustossa saattaa olla käytössä liikaa resursseja, joten sivustomalli ylittää 50 Mega tavun (Mt) rajan.


- Haku saraketta käyttävän luettelon tietojen näyttämisessä on ongelmia. Lisä tietoja on Ohje aiheessa [mallin luoma luettelossa ei näy tietoja oikeista haku luettelosta SharePoint Onlinessa](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Lisä tietoja yleisistä ongelmista ja ratkaisuista on Ohje aiheessa [sivustomallien luominen ja käyttäminen](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

