---
title: Sisältö ei näy hakutuloksissa SharePoint
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: 8215b0a5cde5adffa3bec37d6699418557f914dd
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363800"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>Sisältö ei näy hakutuloksissa SharePoint

Suorita seuraavat vianmääritysvaiheet, kun odotettu sisältö ei näy etsinnän tuloksissa:
  
1. Tarkista, että odotettua sisältöä sisältävä **sivusto** on määritetty sallimaan sisällön näkyvän etsinnän tuloksissa. Noudata [Näytä sisältöä sivuston hakutuloksissa](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).

2. Tarkista, että **luettelo** tai **kirjasto** , joka sisältää odotettu sisältö on sisällön näkyvän etsinnän tuloksissa. Noudata [Näytä sisältöä luetteloiden tai kirjastojen hakutuloksissa](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).

3. Varmista, että sivun, tiedoston tai mukautetun sivun asettelu julkaistaan **pääversio.** Vaiheen 3- [haku ei palauta kaikkia tuloksia SharePoint Onlinessa](https://go.microsoft.com/fwlink/?linkid=874525).

4. Varmista, että käyttäjällä on **oikeudet** tarkastella sisältöä. Ohjeiden [ymmärtäminen käyttöoikeustasoja SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).
    
5. Jos haku rakennetta on muutettu lisäämällä uusi hallittu ominaisuus, hallitun ominaisuuden muokkaamalla tai poistamalla sitten pyytää hallitun ominaisuuden indeksointi ja indeksoida uudelleen vaaditaan. **Indeksoi** sisältö [manuaalisesti pyytää Läpikäymiselle ja indeksoinnille uudelleen sivuston kirjasto tai luettelo](https://docs.microsoft.com/sharepoint/crawl-site-content)-ohjeiden mukaan. Tämä saattaa kestää jonkin aikaa, odota 24 tuntia, ennen kuin tarkistat tulokset uudelleen.

Lisätietoja [voi etsiä tietoja sivuston sisällön käyttöön](https://docs.microsoft.com/sharepoint/make-site-content-searchable). 
  
