---
title: Orpokäyttäjän poistaminen paikallisesta palvelimesta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 7927c0684d2f5289f92506d7d05d5b1a3b43b658
ms.sourcegitcommit: b0b050a83db28566b68e3ec09810c6b94280008e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/20/2020
ms.locfileid: "45198185"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>Orpokäyttäjän poistaminen paikallisesta palvelimesta

Voit poistaa orpokäyttäjän seuraavasti:

1. Pakota hakemistosynkronointi noudattamalla kohdassa [Mikä on yhdistelmäkäyttäjätieto Azure Active Directoryssa?](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories).

2. Lisätietoja hakemistosynkronoinnin tarkistamisesta [on ohjeaiheessa Mikä on azure Active Directoryn yhdistelmäkäyttäjän tunnus?](https://technet.microsoft.com/library/jj151797.aspx).

3. Jos synkronointi toimii oikein, mutta Active Directory -objektin poistaminen ei toimi Azure AD:hen, poista orpoobjekti manuaalisesti jollakin seuraavista Azure Active Directory -moduulin käyttämisestä Windows PowerShell -cmdlet-komentoja varten:

    Poista-MsolContact  
    Poista MsolGroup  
    Poista-MsolUser

    Jos esimerkiksi haluat poistaa orpoja käyttäjätunnuksia john.smith@contoso.com, joka on alun perin luotu hakemistosynkronoinnin avulla, suorita cmdlet-komento:

    Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com