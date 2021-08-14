---
title: AAD-Näyttöyhteys ongelma
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923749"
---
# <a name="problem-with-aad-connect-health"></a>AAD-Näyttöyhteys ongelma

- Varmista, että sinulla on oikeus suorittaa toiminto. Yleiset järjestelmänvalvojat voivat käyttää sitä oletusarvoisesti. Lisäksi voit käyttää roolipohjaista [käyttöoikeuksien hallintaa](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) edustajalle rekisteröintioikeuksien delegoimiseen avustajalle.
- Varmista, että tarvittavat päätepisteet ovat käytössä, eikä niitä ole estetty palomuurin vuoksi. Lisätietoja on [vaatimuksissa.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Rekisteröinti voi epäonnistua, koska verkkokerroksen SSL-tarkastus koskee lähtevää viestintää.
- Varmista, että olet vahvistanut Azure AD:n ilmoitusasetukset Näyttöyhteys kuntoa varten. Tarkista asetus. Tämän [oppaan](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) avulla voit ymmärtää, miten voit määrittää Azure AD:n ilmoitusasetukset Näyttöyhteys kuntoilmoituksia varten.
- Lisätietoja AAD-Näyttöyhteys kuntosynkronointiraportista ja sen lataannista on kohdassa Objektitason [synkronointiraportti.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Jos haluat tehdä AAD-Näyttöyhteys-ilmoitusten vianmäärityksen, noudata [AAD Näyttöyhteys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) Terveystietojen tuoreus -ilmoituksia ja usein kysyttyjä kysymyksiä, katso [AAD:n yleiset Näyttöyhteys kunto-asennusta](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)koskevat kysymykset.
