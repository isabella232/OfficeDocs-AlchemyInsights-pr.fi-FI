---
title: Siirtyminen AIP-ohjelmassa VÄHIMMÄISTUONTIHINNAN/yhdistetyn merkinnän kanssa yhteensopivuus keskuksessa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674323"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Siirtyminen AIP-ohjelmassa VÄHIMMÄISTUONTIHINNAN/yhdistetyn merkinnän kanssa yhteensopivuus keskuksessa

Jos haluat siirtyä AIP-otsikoista tieto turva-ja yhteensopivuus keskuksen yhdenmukaisiin merkintä toimiin, toimi seuraavasti:

**Ota suojaus käyttöön Azure-portaalissa**

1. Jos et ole vielä tehnyt niin, avaa uusi selain ikkuna ja [Kirjaudu sisään Azure-portaaliin](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Siirry **Azure Information Protectionin** terään. Valitse esimerkiksi keskitin-valikossa **Kaikki palvelut** ja ala kirjoittaa **tietoja** suodatin-ruutuun. Valitse **Azure Information Protectionin**. Jos et ole aiemmin käyttänyt Azure Information Protectionin terää, katso [lisä ohjeita](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) tämän lavan lisäämiseen portaaliin. Jos haluat avata Azure Information Protectionin terän, sinulla on oltava joko [Azure Information Protectionin Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) -palvelu paketin tai Office 365-palvelu paketin, joka sisältää oikeuksien hallinnan. Jos sinulla on jokin näistä paketeista, mutta saat ilmoituksen siitä, että kelvollista tilausta ei löydy, [Ota yhteyttä Microsoftin tukeen](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) tai käytä tavallisia tuki kanavia.

2. Etsi **Hallitse** -valikon vaihto ehdot ja valitse **Suojaus aktivointi**. Valitse **Aktivoi**ja vahvista sitten toiminto. Kun Akti vointi on valmis, tieto palkissa näkyy **Akti voinnin onnistuminen**.

**Azure-tieto turva merkintöjen siirtäminen Office 365-suojaus & yhteensopivuus keskukseen**

1. Varmista, että olet kirjautunut sisään käyttäjänä, jolla on yleinen hallinta oikeus.

2. Siirry **Azure Information Protectionin** terään.

3. Valitse **hallinta** -valikko-vaihto ehdossa **yhdistetty merkintä**.

4. Valitse **Azure Information Protectionin yhdistetyn** merkinnän Blade-kohdassa **Aktivoi** ja noudata online-ohjeita.

**Huomautus**: Varmista, että sinulla on tarvittavat käyttö oikeudet, ennen kuin Akti voit suojaus & yhteensopivuus keskuksen siirron. Lisä tietoja on seuraavissa artikkeleissa:

1. [Onko sinun oltava yleinen järjestelmänvalvoja, jotta voit määrittää Azure Information Protectionin tai delegoida sen muille järjestelmänvalvojille?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Tärkeitä tietoja järjestelmänvalvojan rooleista tieto turvaan & yhteensopivuus keskukseen siirryttäessä.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Lisä tietoja AIP:tä yhdistetystä merkintöjen siirtämisestä tieto turva-ja yhteensopivuus keskukseen on kohdassa [tunnisteiden siirtäminen](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
