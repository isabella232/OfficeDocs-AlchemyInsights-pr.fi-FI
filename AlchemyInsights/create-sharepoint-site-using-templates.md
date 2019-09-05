---
title: Sivuston luominen SharePoint Onlinessa
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 42430c8dadc17b87dc7741f3fa045ba7c25fab84
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755305"
---
# <a name="create-sharepoint-sites-using-templates"></a>SharePoint-sivustojen luominen mallien avulla

SharePoint-Sivustomallit ovat ennalta rakennettuja määritelmiä, jotka on suunniteltu tietyn liiketoiminta tarpeen ympärille. Lisä tietoja on kohdassa [mallien käyttäminen erilaisten SharePoint-sivustojen luomiseen](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).

Seuraavassa on joitain yleisiä ongelmia/ratkaisuja, jotka liittyvät sivuston tai luettelon tallentamiseen SharePoint Onlinen mallina. 

**Tallenna sivusto/luettelo malli-painike ei ole käytettävissä tai puuttuu**

Järjestelmänvalvojien on sallittava mukautetun komento sarjan mallin ominaisuuksien ottaminen käyttöön. Tarkempia ohjeita, esimerkkejä ja huomioita on kohdassa 

- [Mukautetun komento sarjan salliminen tai estäminen](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- Tallenna sivusto mallina-komentoa ei tueta, ja se voi aiheuttaa ongelmia sivustoissa, jotka käyttävät SharePoint Serverin Julkaisusinfrastruktuuria.

**Sivustomallia ei voi luoda tai se ei toimi oikein**

Mallista saattaa puuttua [ominaisuus](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , eikä se aktivoida. Jos ominaisuus ei ole käytettävissä nykyisessä sivustokokoelmassa, et voi käyttää sivustomallia sivuston luomiseen.

- Tarkista, ylittyessä luettelot tai kirjastot, jotka ylittävät [luettelo näkymän raja-arvon](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000, koska tämä voi estää sivustomallin luomisen.

- Sivusto saattaa käyttää liikaa resursseja, joten sivustomalli ylittää 50 Mt:N enimmäismäärän.


- Haku saraketta käyttävän luettelon tietojen näyttämiseen liittyy ongelmia. Lisä tietoja on kohdassa [mallin luoma luettelo ei Näytä tietoja oikeasta haku luettelosta SharePoint Onlinessa](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).

Tarkempia tietoja yleisistä ongelmista ja ratkaisuista, tarkista [Luo ja käytä sivustomalleja](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).



