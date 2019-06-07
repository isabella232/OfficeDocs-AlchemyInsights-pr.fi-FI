---
title: Vianmääritys viestit on estetty
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760338"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Käyttö estetty viestit Admin Centerissä Sharepoint/OneDrive liittyviä ongelmia

Jos saat käyttö estetty-sanoman, kun he yrittävät selata Sharepoint-/ OneDrive-hallintakeskukseen, varmista, että et [Määritä käyttöoikeus käyttäjälle](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One). Jos käyttäjällä on käyttöoikeus, sinun olisi myös Varmista, että [määritetty järjestelmänvalvoja-rooli](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , voivat käyttää admin-keskukset ovat.

Tämä ongelma voi ilmetä myös, kun käyttäjä poistetaan ja luodaan uudelleen sama käyttäjätunnus (UPN) kanssa. Uusi tili on luotu käyttämällä eri PUID (yksilöllisen Passport-tunnus)-arvoa. Kun käyttäjä yrittää käyttää sivustokokoelman tai niiden OneDrive, käyttäjällä on virheellinen PUID. Toinen tilanne liittyy directory-synkronointia Active Directoryn organisaatioyksikössä (OU). Jos käyttäjät ovat jo kirjautuneena SharePoint-ovat siirretään eri OU ja SharePointin kanssa resynced, he saattavat kohdata tämän ongelman.

Voit ratkaista tämän ongelman, Palauta alkuperäiset UPN kanssa artikkelin, [Palauta Office 365-käyttäjä](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Huomautus: Jos OneDrive tai SharePoint-Admin center ei ole aikaisemmin olleet tekemisissä useiden käyttäjien käytettävissä, saattaa olla väliaikaista palvelua ongelma.  [Tarkista palvelun terveyden dashboard](https://portal.office.com/adminportal/home#/servicehealth).


