---
title: Korjaa vuokraajakäytäntö (toiminnon ohittaminen)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ee45e86a143719914f7a7917730d7e840e90625f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326794"
---
# <a name="fix-tenant-policy-action-override"></a>Korjaa vuokraajakäytäntö (toiminnon ohittaminen)

Jokin roskapostin estokäytännöistäsi vaikuttaa tähän viestiin. Voit tarkistaa käytännöt seuraavasti:

1. Siirry Microsoft 365 Defender -portaalissa kohtaan <https://security.microsoft.com/> **Sähköposti- &-&** \> **Käytännöt-kohdassa** Sääntöjen uhkien käytännöt roskapostin \>  \>  esto. 

   Jos haluat siirtyä suoraan **Roskapostin käytännöt -sivulle,** käytä <https://security.microsoft.com/antispam> -

2. Valitse **roskapostikäytännöt** -sivulla käytäntö napsauttamalla käytännön nimeä ( Tyyppi on Mukautettu  roskapostin estokäytäntö tai Nimi roskapostin estokäytäntö **(oletus).** 
3. Valitse näyttöön tulevassa tietojen pikaikkunassa Muokkaa **toimintojaToiminnot-osassa.** 
4. Tarkista **Viestitoiminnot-osassa** Roskaposti-, Luotettava roskaposti-, Tietojen kalastelu- ja Tietokalastelu-vaihtoehdot ja Tarkista, onko jokin seuraavista arvoista valittuna:   
   - **X-otsikon lisääminen**
   - **Prepend subject line with text**
   - **Viestin uudelleenohjaus sähköpostiosoitteeseen**
   - **Poista viesti**
   - **Ei toimia**

   On mahdollista, että **vakioasetuksia sovelletaan kaikkiin** Exchange Online Protection vaikuttaa viestiin.

Lisätietoja on kohdassa [Roskapostin estokäytäntöjen määrittäminen EOP:ssä.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)
