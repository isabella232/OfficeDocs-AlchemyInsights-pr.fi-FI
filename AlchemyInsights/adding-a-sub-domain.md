---
title: Alitoimialueen lisääminen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506488"
---
# <a name="adding-a-sub-domain"></a>Alitoimialueen lisääminen

Alitoimialue voidaan lisätä samaan tai eri vuokraajaan kuin päätoimialue. Kummassakin tapauksessa sinun on hallittava omia DNS-asetuksiasi rekisteröijän sivustossa. Jos olet sallinut Microsoftin hallita DNS-asetuksiasi NS-tietueilla tai jos ostit toimialueen Microsoftilta, et voi lisätä alitoimialueita muuttamatta tätä ensin.

Lisää ensin päätoimialue ja lisää sitten alitoimialue. Jos alitoimialue on samassa vuokraajassa, lisävahvistus ei ole tarpeen. Jos lisäät alitoimialueen erilliseen vuokraajaan, omistajuuden vahvistusta varten tarvitaan DNS-txt-tietue ennen toimialueen lisäämistä ja valittujen palveluiden MUITA DNS-tietueita.

- Jos haluat lisätä toimialueen tai alitoimialueen, noudata ohjattua Toimialueen lisääminen -toimintoa tai lisää toimialue tai alitoimialue manuaalisesti valitsemalla **Toimialueen** lisääminen [](https://admin.microsoft.com/Adminportal#/Domains/Wizard)  >    >  **toimialueiden lisääminen**.

Tarvittaessa:

- Jos haluat muuttaa olemassa olevan toimialueen DNS-asetusten hallintaa, siirry kohtaan **Asetukset** Toimialueet, valitse toimialueen vieressä oleva valintaruutu ja  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)valitse sitten **DNS-hallinta.** Valitse ohjatussa toiminnossa **Lisää omat DNS-tietueet** ja suorita ohjattu toiminto loppuun.
- Jos haluat lisätä alitoimialueita Microsoftin ostamaan toimialueeseen, siirrä toimialue ensin toiseen rekisteröintipalveluun ja tee sitten yllä oleva muutos, jotta voit hallita omia DNS-tietueitasi. Katso ohjeet ohjeesta [Toimialueen siirtäminen Microsoftista toiseen isäntään.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)
- Jos saat virheilmoituksen, että toimialueesi on jo muiden organisaatiosi jäsenten tai muiden organisaation jäsenten käytössä, sinun on ensin otettava tämä hallitsematon tili hallintaasi varten ennen toimialueen käyttöä. Katso ohjeet artikkelista [Hallitsemattoman hakemiston hallinta järjestelmänvalvojana](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover)Azure Active Directory.
