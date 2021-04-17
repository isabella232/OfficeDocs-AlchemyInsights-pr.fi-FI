---
title: Siirtyminen AIP:stä MIP:ksi tai yhdistetyksi osoitetarrojen siirroksi yhteensopivuuskeskuksessa
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825368"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Siirtyminen AIP:stä MIP:ksi tai yhdistetyksi osoitetarrojen siirroksi yhteensopivuuskeskuksessa

Jos haluat siirtyä AIP-selitteet yhdistettyyn osoitetarraan tietoturva- ja yhteensopivuuskeskuksessa, tee näin:

**Suojauksen aktivoiminen Azure-portaalista**

1. Jos et ole vielä tehnyt niin, avaa uusi selainikkuna ja kirjaudu [sisään Azure-portaaliin.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal) Siirry **Azure Information Protection -teriin.** Valitse esimerkiksi keskusvalikossa Kaikki palvelut **ja ala** kirjoittaa Tiedot Suodatin-ruutuun.  Valitse **Azure Information Protection**. Jos et ole ennen käynyt Azure Information Protection -osaa, [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) katso ohjeet tämän terien lisäämiseksi portaaliin kertakäyttöisillä lisävaiheilla. Jotta voit avata Azure Information Protection -laikan, sinulla on oltava [joko Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) -palvelupaketti tai Office 365 -palvelupaketti, joka sisältää oikeuksien hallinnan. Jos sinulla on jokin näistä tilauksia, mutta näet viestin, jonka mukaan kelvollista tilausta ei löydy, ota yhteyttä [Microsoft-tukeen](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) tai käytä vakiotukikanaviasi.

2. Etsi **Hallinta-valikkovaihtoehdot** ja valitse **Suojausaktivointi**. Valitse **Aktivoi** ja vahvista sitten toiminto. Kun aktivointi on valmis, tietopalkissa näkyy teksti Aktivointi **suoritettu.**

**Azure Information Protection -tunnisteiden siirtäminen Office 365:n & yhteensopivuuskeskukseen**

1. Varmista, että olet kirjautunut sisään käyttäjänä yleisenä järjestelmänvalvojana.

2. Siirry **Azure Information Protection -teriin.**

3. Valitse **Hallinta-valikkovaihtoehdosta** **Yhdistetty selite**.

4. Valitse **Azure Information Protection - Unified Labeling -laitteessa** **Aktivoi** ja noudata online-ohjeita.

**Huomautus:** Varmista, että sinulla on tarvittavat käyttöoikeudet ennen tietoturvakeskuksen & aktivoimista. Lisätietoja on näissä artikkeleissa:

1. [Onko sinun oltava yleinen järjestelmänvalvoja Azure Information Protectionin määrittämiseksi vai voinko delegoida sen muille järjestelmänvalvojille?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Tärkeitä tietoja järjestelmänvalvojan rooleista tietoturva- ja & jälkeen.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Lisätietoja AIP:n yhdistetyn osoitetarrojen siirrosta tietoturva- ja yhteensopivuuskeskukseen on kohdassa [Osoitetarrojen siirtäminen.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)
