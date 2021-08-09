---
title: 'AIP: Käytännöt eivät toimi odotetulla tavalla'
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
- "9002266"
- "4780"
ms.openlocfilehash: 90448bf57297ce59ba222efd1927b5de588bfbfdb1206b6403764d7f43fed690
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934290"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Käytännöt eivät toimi odotetulla tavalla

Azure Information Protection: Käytännöt eivät toimi odotetulla tavalla, katso seuraavista ohjeista eri käytäntöihin liittyviä ohjeita:

1. Jos visuaalisissa merkinnöissä on ongelmia, lue kohta [Kun visuaalisia merkintöjä käytetään](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Jos sinulla on ongelmia automaattisen otsikoinnin kanssa, lue ohjeet automaattisen ja suosittelun luokittelun määrittämiseen [Azure Information Protectionille](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ja Mitä luottamukselliset [tietotyypit etsivät](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Jos sinulla on ongelmia alkuperäisen/Pfile-suojauksen kanssa, tarkista Tiedoston [ohjelmointirajapinnan määritykset.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)
4. Tarkista, käytätkö kohdistettuja käytäntöjä, joita ei ole määritetty oikein: [Azure Information Protection -käytännön määrittäminen tietyille käyttäjille kohdistettujen käytäntöjen avulla](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Jos automaattinen selite ei toimi Outlook kun liität osoitetarroja, varmista, että DRMEncryptProperty-funktiota ei ole määritetty seuraavassa kuvatulla tavalla: [IRM-rekisteriasetukset suojausta varten.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)

Jos ongelmia ilmenee edelleen, kerää Azure Information Protection -asiakaslokit ja liitä viedyt lokit tähän lippuun.

1. Avaa Office-tiedosto tai luo uusi sähköpostiviesti Outlookissa.
2. Valitse **Suojaus ja luottamuksellisuus** > **Ohje- ja palaute**.
3. Valitse **Vie lokit**.
4. Tallenna lokit sijaintisi mukaan ja liitä ne tähän palvelupyyntöön.

Lisäresursseja:

- [Otsikon määrittäminen visuaalisia merkintöjä varten Azure Information Protectionissa](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Tutustu Azure Information Protection -ohjeisiin](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Luottamuksellisuusotsikoiden käyttäminen Microsoft 365 sovelluksissa](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

