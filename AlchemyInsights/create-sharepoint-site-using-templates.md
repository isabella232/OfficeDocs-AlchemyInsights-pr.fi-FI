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
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732217"
---
# <a name="create-sharepoint-sites-using-templates"></a>SharePoint-sivuston luominen mallien avulla

Modernia viestintää tai ryhmä sivustoja ei voi käyttää sivuston tallentamiseen mallina. Lisä tietoja mallien käyttämisestä on Ohje aiheessa [SharePoint-sivuston tallentaminen, lataaminen ja lataaminen mallina](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).

Seuraavassa on joitakin yleisiä ongelmia tai ratkaisuja, jotka liittyvät sivuston tai luettelon tallentamiseen SharePoint Onlinen mallina. 

**Tallenna sivuston/luettelon malli-painike ei ole käytettävissä tai se puuttuu**

Järjestelmänvalvojien on sallittava malli ominaisuuksien käyttöönotto mukautetulla komento sarjalla. Yksityiskohtaisia ohjeita, esimerkkejä ja Huomioitavaa 

- [Mukautetun komento sarjan salliminen tai estäminen](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Tallenna sivusto mallina-komento ei ole käytettävissä, ja se voi aiheuttaa ongelmia SharePoint Serverin Julkaisuinfrastruktuuria käyttävien sivustojen kanssa.

**Sivustomallia ei voi luoda tai se ei toimi oikein**

Mallista saattaa puuttua [ominaisuus](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , eikä se aktivoidu. Jos ominaisuus ei ole käytettävissä nykyisessä sivustokokoelmassa, sivustomallia ei voi käyttää sivuston luomiseen.

- Tarkista, ylittävätkö luettelot tai kirjastot 5000-kohteiden [luettelo näkymän raja-arvon](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) , sillä tämä voi estää sivustomallin luomisen.

- Sivustossa saattaa olla käytössä liikaa resursseja, joten sivustomalli ylittää 50 Mt: n rajan.


- Haku saraketta käyttävän luettelon tietojen näyttämisessä on ongelmia. Lisä tietoja on Ohje aiheessa [mallin luoma luettelossa ei näy tietoja oikeista haku luettelosta SharePoint Onlinessa](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Jos haluat lisä tietoja yleisistä ongelmista ja ratkaisuista, valitse [sivustomallien luominen ja käyttäminen](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



