---
title: Sivuston poistaminen pysyvästi SharePointissa
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: f461963c4a5719957258349d667731231023721ab3ee4641538c94371bf3f56d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53944308"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a>Sivuston poistaminen pysyvästi SharePointissa

Jos haluat käyttää poistettuun sivustoon liittyvää URL-osoitetta uudelleen (sivuston uudelleenluomiseen) tai poistaa sivuston pysyvästi, koska sitä ei enää käytetä, voit käyttää uuden SharePoint-hallintakeskuksen **Poista pysyvästi** -toimintoa. 

1. Siirry [uuden SharePoint-hallintakeskuksen poistettujen sivustojen sivulle ](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) ja kirjaudu sisään tilillä, jolla on organisaatiosi järjestelmänvalvojan oikeudet. 

2. Valitse vasemmassa sarakkeessa sivusto. 

3. Napsauta **Poista pysyvästi**. 

**Huomautus**: ryhmään yhdistettyjä sivustoja ei voi poistaa pysyvästi uudesta SharePoint-hallintakeskuksesta. Käytä sen sijaan cmdlet-komentoa [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite).  

Lisätietoja on artikkelissa [Sivuston poistaminen pysyvästi](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site). 
