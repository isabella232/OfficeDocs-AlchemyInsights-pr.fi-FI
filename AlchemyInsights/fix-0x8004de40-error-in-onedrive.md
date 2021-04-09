---
title: OneDriven 0x8004de40-virheen korjaus
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649745"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>OneDriven 0x8004de40-virheen korjaus

Jos käyttöjärjestelmäsi on Windows 7 ja saat tämän virheilmoituksen, [TLS 1.1- ja TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)-protokollat otetaan käyttöön Windows-käyttöjärjestelmän WinHTTP -käyttöjärjestelmän oletusarvoisen suojatun protokollan päivityksen avulla.

Jos käytössäsi on Windows 10 ja saat virheilmoituksen 0x8004de40 OneDrivesta:

- Käynnistä tietokone uudelleen, kun yhteys Acitve-hakemistotoimialueeseen on muodostettu.
- Jos uudelleenkäynnistys ei korjaa ongelmaa, poista laitteen kiinnitys ja lisää se uudelleen Azure AD:stä. 

**Huomautus:** sinun pitäisi olla yrityksen verkossa, kun suoritat näitä vaiheita. Älä suorita näitä vaiheita, kun et ole yhteydessä yrityksen infrastruktuuriin (esimerkiksi matkustaessasi). 

1. Avaa järjestelmänvalvojan oikeuksin suoritettava **komentokehote valitsemalla Käynnistä**, napsauttamalla **komentokehotetta** hiiren kakkospainikkeella ja valitsemalla sitten **Suorita järjestelmänvalvojana**.

1. Kirjoita *dsregcmd /leave ja paina* **Enter-näppäintä.**

1. Kun olet valmis, kirjoita *dsregcmd /join ja paina* **Enter-näppäintä.**

1. Kun olet valmis, sulje komentokehote.

1. Käynnistä tietokone uudelleen ja kirjaudu OneDriveen.