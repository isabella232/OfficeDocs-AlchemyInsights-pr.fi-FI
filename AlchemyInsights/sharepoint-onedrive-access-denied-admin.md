---
title: Estettyjen viestien käytön vianmääritys
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758428"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Estettyjen viestien vianmääritys Sharepointissa tai OneDrive-hallintakeskuksessa

Jos näyttöön tulee käyttöestetty-sanoma, kun yrität selata Sharepoint/OneDrive-hallintakeskusta, varmista, että [määrität käyttäjälle käyttöoikeuden.](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One) Jos käyttäjällä on käyttöoikeus, varmista myös, että hänelle [on määritetty järjestelmänvalvojan rooli,](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) joka voi käyttää hallintakeskuksia.

Tämä ongelma voi ilmetä myös silloin, kun käyttäjä poistetaan ja luodaan uudelleen samalla käyttäjänimellä (UPN). Uusi tili luodaan käyttämällä toista PUID (Passport Unique ID) -arvoa. Kun käyttäjä yrittää käyttää sivustokokoelmaa tai OneDrivea, käyttäjällä on virheellinen PUID-tunnus. Toinen skenaario koskee hakemistosynkronointia Active Directory -organisaatioyksikön kanssa. Jos käyttäjät ovat jo kirjautuneet SharePointiin ja siirretään sitten toiseen organisaatioyhteisöön ja synkronoidaan uudelleen SharePointin kanssa, he saattavat kohdata tämän ongelman.

Voit ratkaista tämän ongelman palauttamalla alkuperäisen UPN:n noudattamalla artikkelin [Palauta käyttäjä Microsoft 365 :ssä](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)ohjeita.

Huomautus: Jos OneDrive- tai SharePoint-hallintakeskus ei ole useiden käyttäjien käytettävissä, joilla on aiemmin ollut käyttöoikeus, palveluongelma saattaa olla tilapäinen.  [Tarkista palvelun kunnon koontinäyttö](https://portal.office.com/adminportal/home#/servicehealth).


