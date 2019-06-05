---
title: Suorituskyvyn ongelmat-SharePoint- tai OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719514"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint- tai OneDrive on hidas tai ei voi käyttää useita käyttäjiä

Jos OneDrive tai SharePoint-sivustossa ei ole aikaisemmin olleet tekemisissä useiden käyttäjien käytettävissä, saattaa olla väliaikaista palvelua ongelma. [Tarkista palvelun terveyden dashboard](https://portal.office.com/adminportal/home#/servicehealth).

## <a name="add-and-license-the-user"></a>Lisää ja anna käyttäjän

Varmista, että voit [määrittää käyttöoikeuksia käyttäjille Office 365 yrityksille](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).


## <a name="assign-permissions"></a>Käyttöoikeuksien määrittäminen

Jos käyttäjä on määritetty Sharepoint-käyttöoikeus ja silti saa käyttö estetty-sanoman, varmista, että ne on määritetty [asianmukaisen käyttöoikeustason](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) .

## <a name="consider-using-the-access-request-feature"></a>Harkitse access request-toiminnolla

[Access request-ominaisuus](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) sallii käyttäjät voivat käyttää sisältöä, joka ei tällä hetkellä heillä on oikeus pyytää.

## <a name="allow-custom-script-may-cause-access-denied-issues"></a>Salli mukautetun komentosarjan voi aiheuttaa ongelmia ei ole käyttöoikeutta

On tiettyjä tilanteita, jossa *Salli mukautetun komentosarjan* ominaisuus voi olla esittämisen käyttö estetty. Seuraavat ominaisuudet muuttuvat, luettelo, tietojen suojaus ja ominaisuus poistetaan käytöstä. Vieraile osoitteessa [Salli tai estä mukautetun komentosarjan](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).

