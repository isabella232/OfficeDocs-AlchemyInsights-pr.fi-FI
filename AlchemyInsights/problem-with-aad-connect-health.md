---
title: Ongelma AAD Connect Healthissa
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
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481466"
---
# <a name="problem-with-aad-connect-health"></a>Ongelma AAD Connect Healthissa

- Varmista, että sinulla on oikeus suorittaa toiminto. Yleiset järjestelmänvalvojat voivat käyttää sitä oletusarvoisesti. Lisäksi roolipohjaisen käyttöoikeuksien [hallinnan avulla voit delegoida](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) rekisteröintioikeudet avustajalle.
- Varmista, että tarvittavat päätepisteet ovat käytössä eikä niitä ole estetty palomuurin vuoksi. Lisätietoja on [vaatimuksissa.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Rekisteröinti voi epäonnistua, koska verkkokerroksen kautta lähtevien yhteyksien SSL-tarkastus koskee.
- Varmista, että olet vahvistanut Azure AD Connect Healthin ilmoitusasetukset. Tarkista asetus. Tämän [oppaan](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) avulla voit ymmärtää, miten voit määrittää Azure AD Connectin kuntoilmoitusten ilmoitusasetukset.
- Lisätietoja AAD Connect Health -synkronointiraportista ja sen lataannista on objektitason [synkronointiraportissa.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Jos haluat tehdä AAD Connect Health -ilmoitusten vianmäärityksen, katso [AAD Connect Healthin](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) tietojen tuoreusilmoituksia ja usein kysyttyjä kysymyksiä koskevat vianmääritysohjeet [AAD Connect Healthin asennusta varten.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)
