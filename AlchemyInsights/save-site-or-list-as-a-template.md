---
title: Tallenna sivusto tai luettelo mallina
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 627f49991aaef984f731412045351d7a1862b376
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048721"
---
# <a name="save-site-or-list-as-a-template"></a>Tallenna sivusto tai luettelo mallina

SharePoint-Sivustomallit ovat ennalta rakennettuja määritelmiä, jotka on suunniteltu tietyn liiketoiminta tarpeen ympärille. Lisä tietoja on kohdassa [mallien käyttäminen erilaisten SharePoint-sivustojen luomiseen](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Seuraavassa on joitain yleisiä ongelmia/ratkaisuja, jotka liittyvät sivuston tai luettelon tallentamiseen SharePoint Onlinen mallina.

**Tallenna sivusto/luettelo malli-painike ei ole käytettävissä tai puuttuu**. 

- Järjestelmänvalvojien on sallittava mukautetun komento sarjan mallin ominaisuuksien ottaminen käyttöön. Yksityiskohtaisia ohjeita, esimerkkejä ja huomioitavia seikkoja on kohdassa [mukautetun komento sarjan salliminen tai estäminen](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).


- Tallenna sivusto mallina-komentoa ei tueta, ja se voi aiheuttaa ongelmia sivustoissa, jotka käyttävät SharePoint Serverin Julkaisusinfrastruktuuria.


**Sivustomallia ei voi luoda tai se ei toimi oikein**

- Mallista saattaa puuttua [ominaisuus](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , eikä se aktivoida. Jos ominaisuus ei ole käytettävissä nykyisessä sivustokokoelmassa, et voi käyttää sivustomallia sivuston luomiseen.


- Tarkista, ylittyessä luettelot tai kirjastot, jotka ylittävät [luettelo näkymän raja-arvon](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000, koska tämä voi estää sivustomallin luomisen.


- Sivusto saattaa käyttää liikaa resursseja, joten sivustomalli ylittää 50 Mega tavun (Mt) rajan.


- Haku saraketta käyttävän luettelon tietojen näyttämiseen liittyy ongelmia. Lisä tietoja on kohdassa [mallin luoma luettelo ei Näytä tietoja oikeasta haku luettelosta SharePoint Onlinessa](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).


Tarkempia tietoja yleisistä ongelmista ja ratkaisuista saat Ohje kirjasta, [luoda ja käyttää sivustomalleja](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).

