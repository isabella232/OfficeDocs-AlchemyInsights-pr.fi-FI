---
title: Käyttö estetty-viestien vian määritys
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767659"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Käyttö estetty-viestien vian määritys SharePoint/OneDrive-hallinta keskuksessa

Jos vastaanotat käyttö estetty-viestin, kun yrität siirtyä SharePoint/OneDrive-hallinta keskukseen, varmista, että määrität [käyttäjälle käyttö oikeuden](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Jos käyttäjällä on käyttö oikeus, Varmista myös, että [hänelle on määritetty järjestelmänvalvojan rooli](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) , joka voi käyttää hallinta keskuksia.

Tämä ongelma voi ilmetä myös silloin, kun käyttäjä poistetaan ja luodaan uudelleen käyttäen samaa käyttäjän päänimeä (UPN). Uusi tili luodaan käyttämällä toista PUID (Passport Unique ID)-arvoa. Kun käyttäjä yrittää käyttää sivustokokoelmaa tai OneDrivea, käyttäjällä on virheellinen PUID. Toinen skenaario sisältää hakemisto synkronoinnin Active Directoryn organisaatio yksikön (OU) kanssa. Jos käyttäjä on jo kirjautunut SharePointiin ja siirtyy sitten toiseen organisaatio yksikköön ja on siirretty SharePointiin, ongelma saattaa ilmetä.

Voit korjata ongelman palauttamalla alkuperäisen UPN:N artikkelin ohjeiden mukaisesti ja [palauttamalla käyttäjän Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)-sovelluksessa.

Huomautus: Jos OneDrive-tai SharePoint-hallinta keskus ei ole käytettävissä useille käyttäjille, joilla on aiemmin ollut käyttö oikeus, kyseessä saattaa olla tilapäinen palvelu ongelma.  [Tarkista palvelun kunnon koonti näyttö](https://portal.office.com/adminportal/home#/servicehealth).


