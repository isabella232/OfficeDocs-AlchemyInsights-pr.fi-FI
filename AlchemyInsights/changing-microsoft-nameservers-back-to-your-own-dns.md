---
title: Microsoftin nimipalvelimien vaihtaminen takaisin omien DNS-tietueiden hallintaan
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506603"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Microsoftin nimipalvelimien vaihtaminen takaisin omien DNS-tietueiden hallintaan

Olet aiemmin muuttanut nimipalvelintietueet Microsoftiin (ns1.bdm.microsoftonline.com), mutta olet nyt päättänyt hallita omia DNS-tietueitasi:

Muuta nimipalvelin takaisin rekisteröintipalveluun tai edelliseen asetukseen toimialuerekisteröijän sivustossa. Jos et tunne DSN-asetuksia, ota yhteyttä toimialuerekisteröintipalvelusi tukeen. Huomaa, että nimipalvelimen muutosten välittyminen voi kestää jopa 48 tuntia. 

1. Siirry Microsoft 365 hallintaportaalissa kohtaan **Asetukset** Toimialueet, valitse toimialueen vieressä olevaa valintaruutua  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)ja valitse **DNS-hallinta.** 

2. Valitse ohjatussa toiminnossa **Lisää omat DNS-tietueet** ja suorita ohjattu toiminto loppuun. Tämä muuttaa DNS-hallintaa ja mahdollistaa sen, että voit lisätä mukautettuja DNS-tietueita, jotka tarvitaan valittujen palvelujen tueksi.

Jos olet muuttanut nimipalvelintietueet Microsoftiin ja sinulla on sivusto, voit lisätä sivustoon DNS-tietueet nimipalvelimien takaisin muuttamisen sijaan. Lisätietoja on kohdassa [DNS-tietueiden päivittäminen sivuston säilytystä varten nykyisessä isännöintipalvelussa.](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)


