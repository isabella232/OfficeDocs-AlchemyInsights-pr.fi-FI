---
title: Järjestelmänvalvojien lisääminen ja hallinta
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7424"
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755436"
---
# <a name="how-to-add-and-manage-admins"></a>Järjestelmänvalvojien lisääminen ja hallinta

Ongelman kuva uksen perusteella olemme löytäneet ratkaisun. Useimmat Asiakkaat pystyivät ratkaisemaan ongelmaansa sen jälkeen, kun he ovat seuraavat asia kirjojamme.

Jos haluat hallita Microsoft-asiakas sopimusta (MCA), voit käyttää eri rooleja, joilla on haluttu käyttö oikeus taso. Nämä roolit ovat niiden sisäisten Azure-palvelu roolien lisäksi, joiden avulla voit hallita resurssejasi.

**Voit lisätä laskutus rooleja Azure-portaalissa seuraavasti:**

1. Kirjaudu sisään Azure- [portaaliin](https://portal.azure.com/).
2. Hae *kustannusten hallinta + laskutus*.
3. Valitse käytön hallinta (IAM) sellaisen käyttö alueen mukaan, kuten laskutus tili, laskutus profiili tai laskun osa, jossa haluat myöntää käyttö oikeuden.
4. Käyttö oikeuksien hallinta-sivulla on lueteltu käyttäjät ja ryhmät, jotka on määritetty kullekin roolille kyseiselle alueelle.
5. Jos haluat antaa käyttäjälle käyttö oikeuden, valitse **Lisää** sivun yläreunasta. Valitse rooli avattavasta *rooli* -luettelosta. Kirjoita sen käyttäjän Sähkö posti osoite, jolle haluat myöntää käyttö oikeuden. Määritä rooli valitsemalla **Tallenna** .
6. Jos haluat poistaa käyttäjän käyttö oikeuden, valitse käyttäjä, jonka rooli määritystä haluat poistaa. Valitse **Poista**.

**Suositellut asiakirjat**

- [Laskutus rooli määritykset](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [Laskutus tilin roolit ja tehtävät](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [MCA-laskutus tilin käytön aloittaminen](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [Microsoft-asiakas sopimuksen käytön tarkistaminen](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
