---
title: Työn kulku ei käynnistyi
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: cf7bd95e9a8f1d0842f0abcf82c758d649e80c0f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049334"
---
# <a name="workflow-is-not-starting"></a>Työn kulku ei käynnistyi

- SharePoint 2010 ja SharePoint 2013-työn kulut eivät käynnistyi.

    - Jos työn kulku ei ole käynnistyminen, saattaa olla tilapäinen palvelu ongelma, jossa käyttäjät saattavat kohdata ajoittaisia viiveitä työn kulun edistymisen kanssa. Tarkista [palvelun kunnon koonti näytöstä](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , onko organisaatiossasi vaikutusta.

    - Jos tämän ongelman ensimmäisen näkemis kerran jälkeen on kulunut yli 24 tuntia, kirjaudu tuki lippuun. Monissa tapa uksissa olemme jo tekemässä ratkaisua. Ole hyvä ja anna meille vähintään 24 tuntia aikaa ratkaisun suorittamiseen.

- SharePoint 2010-työn kulut viivästyivät käynnistyksen jälkeen.

    - Näin tapahtuu, jos työn kulku käynnistetään suurissa erissä. (esimerkiksi kun useita kohteita lisätään kerralla).

    - Työn kulkuja ei ole suunniteltu suorittamaan reaaliaikaista toimintaa, joten viive on suunnittelun mukaan suoritettava.

   -  Jos työn kulku on monimutkainen XMOL (Extensible Object Markup Language)-kieli, kääntäminen voi olla hidasta. Tarkista [Tämä](https://support.microsoft.com//kb/3043697) artikkeli.

    - Yksinkertaista työn kulkua tai Suunnittele se uudelleen käyttämällä Microsoft SharePoint 2013-työn kulku ympäristön tyyppiä.

    - Jos työn kulku historiasi on kasvanut suureksi, haluat ehkä tyhjentää kohteet tai luoda uuden historia luettelon.

        Lisä tietoja: [työn kulku historian Tyhjentuminen](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Aiheeseen liittyvät artikkelit
Haluatko kokeilla Microsoft Flow'ta SharePoint Onlinessa?
- [Luo työn kulku](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint ja Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


