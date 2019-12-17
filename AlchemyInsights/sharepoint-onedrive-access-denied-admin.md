---
title: Käyttö estetty-sanomien vian määritys
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 57919e6dbd81a5bf3b17fb067485e8eec23b7d4c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051422"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>SharePoint/OneDrive-hallinta keskuksen käyttö estetty-viestien vian määritys

Jos saat käyttö estetty-sanoman yritettäessä selata SharePoint/OneDrive-hallinta keskukseen, varmista, että määrität [käyttäjälle](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)käyttö oikeuden. Jos käyttäjällä on käyttö oikeus, Varmista myös, että heille on [määritetty järjestelmänvalvojan rooli](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , joka voi käyttää hallinta keskuksia.

Tämä ongelma voi ilmetä myös, kun käyttäjä poistetaan ja luodaan uudelleen samalla käyttäjä nimellä (UPN). Uusi tili luodaan käyttämällä eri PUID (Passport Unique ID)-arvoa. Kun käyttäjä yrittää käyttää sivustokokoelmaa tai OneDrivea, käyttäjällä on väärä PUID-tunnus. Toinen skenaario koskee hakemiston synkronointia Active Directory-organisaatio yksikön (OU) kanssa. Jos käyttäjät ovat jo kirjauduneet sisään SharePointiin ja ne siirretään toiseen kohteeseen ja synkronoidaan SharePointin kanssa, ongelma saattaa ilmetä.

Voit ratkaista tämän ongelman palauttamalla alkuperäisen käyttäjä tieto järjestelmän artikkelin ohjeiden mukaisesti, [palauttamalla käyttäjän Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).

Huomautus: Jos OneDrive tai SharePointin hallinta keskus ei ole usean sellaisen käyttäjän käytettävissä, joilla on aiemmin ollut käyttö oikeus, kyseessä voi olla tilapäinen palvelu ongelma.  [Tarkista palvelun kunnon koonti näyttö](https://portal.office.com/adminportal/home#/servicehealth).


