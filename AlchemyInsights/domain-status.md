---
title: Toimialueen tila – Ei palveluita valittuna
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 1476a88c7b974a9e6cfe443f6842df8cdc3d7073a73c0add7e6f183dd0528de1
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57874392"
---
# <a name="domain-status---no-services-selected"></a>Toimialueen tila – Ei palveluita valittuna

**Ei valittuja** palveluita tarkoittaa, että et ole valinnut mitään Microsoft 365-palveluita, kuten Exchange Online Skype for Business tai Intunea, Microsoft 365 mobiililaitteiden hallintaa mukautettua toimialuetta varten. Jos käytät Exchange yhdistelmäympäristöä (Exchange, jossa on Exchange Online) tai ulkoista roskapostisuodatusta Exchange eikä muita Microsoft-palvelut, voit ohittaa tämän viestin. Toimialueen kunto on käytettävissä vain toimialueissa, jotka on yhdistetty suoraan palveluun.

Voit valita toimialueesi palvelut toimilla toimilla:

1. Valitse **Asetukset**  >  [**Toimialueet**](https://admin.microsoft.com/Adminportal/Home)-kohdassa sen toimialueen vieressä olevaa valintaruutua, jossa **tilailmoituksena Ei palveluita on valittuna.**
1. Käynnistä **ohjattu toimialueen määritystoiminto** valitsemalla DNS-hallinta.
    - Jos valitset **Lisää omia DNS-tietueita**, muista valita palvelu pyydettäessä. Lisäasetukset-kohdassa voi olla **lisää palveluja.**
    - Jos valitset Anna **Microsoftin lisätä DNS-tietueet tai** **Lisää** asetuksia Määritä online-palvelut minulle kaikki käytettävissä olevat palvelut, ehdotetaan  >   ja valitaan automaattisesti.
1. Suorita DNS-määritys ja palveluvalinnat loppuun ohjatun toiminnon avulla.
 
Lisätietoja toimialueen määrittämisestä on kohdassa [DNS-tietueiden lisääminen toimialueen liittämistä varten.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)

