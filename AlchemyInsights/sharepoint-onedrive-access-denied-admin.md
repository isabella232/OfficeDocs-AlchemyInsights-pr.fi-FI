---
title: Käyttö estettyjen viestien vianmääritys
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707951"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Käyttö estettyjen viestien vianmääritys SharePoint- tai OneDrive-hallintakeskuksessa

Jos näyttöön tulee käyttö estetty -sanoma, kun yrität selata SharePoint- tai OneDrive-hallintakeskukseen, varmista, että määrität [käyttäjälle käyttöoikeuden.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Jos käyttäjällä on käyttöoikeus, varmista myös, [](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) että käyttäjälle on määritetty järjestelmänvalvojan rooli, joka voi käyttää hallintakeskuksia.

Tämä ongelma voi ilmetä myös silloin, kun käyttäjä poistetaan ja luodaan uudelleen samalla käyttäjätunnuksilla (UPN). Uusi tili luodaan käyttämällä eri PUID (Passport Unique ID) -arvoa. Kun käyttäjä yrittää käyttää sivustokokoelmaa tai OneDrivea, käyttäjällä on virheellinen PUID. Toinen skenaario koskee hakemistosynkronointia Active Directory -organisaatioyksikön (OU) kanssa. Jos käyttäjät ovat jo kirjautuneet SharePointiin ja heidät siirretään toiseen ou:han ja synkronoidaan uudelleen SharePointin kanssa, he saattavat kokea tämän ongelman.

Voit ratkaista tämän ongelman palauttaen alkuperäisen käyttäjätunnuksen artikkelin Palauta käyttäjä [Microsoft 365:ssä ohjeiden mukaisesti.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)

Huomautus: Jos OneDrive- tai SharePoint-hallintakeskus ei ole käytettävissä useille käyttäjille, joilla oli aiemmin käyttöoikeus, voi olla tilapäinen palveluongelma.  [Tarkista palvelun kunto -koontinäyttö.](https://portal.office.com/adminportal/home#/servicehealth)


