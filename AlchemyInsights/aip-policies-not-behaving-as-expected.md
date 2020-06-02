---
title: 'AIP: Käytännöt eivät toimi odotetusti'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 527556fcb02525eb88ea992c38a2ddfcba6f9453
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506555"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: Käytännöt eivät toimi odotetusti

Azure-tietojen suojaus: Käytännöt eivät toimi odotetulla tavalla, katso seuraavat suositellut ohjeet eri käytäntöon liittyville kysymyksille:

1. Jos sinulla on ongelmia visuaalisten merkintöjen kanssa, tutustu [kun visuaalisia merkintöjä käytetään](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).
2. Jos automaattisessa merkintöjen yhteydessä on ongelmia, tutustu [azure-tietojen suojauksen automaattisen ja suositellun luokituksen ehtojen määrittämiseen](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ja [mitä arkaluonteiset tietotyypit etsivät](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
3. Jos sinulla on ongelmia Native/Pfile-suojauksen kanssa, tutustu [Tiedoston API-kokoonpanoon](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Tarkista, käytätkö vaikutusaluekäytäntöjä, joita ei ole määritetty oikein: [Azure Information Protection -käytännön määrittäminen tietyille käyttäjille vaikutusaluekäytäntöjen avulla](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Jos automaattinen merkintä ei toimi Outlookissa, kun liität merkittyä asiakirjaa, varmista, että DRMEncryptProperty-tiedostoa ei ole määritetty tässä kuvatulla tavalla: [IRM-rekisteriasetukset suojausta varten](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Jos ongelmat jatkuvat, kerää Azure Information Protection -asiakaslokit ja liitä viedyt lokit tähän lippuun.

1. Avaa Office-asiakirja tai luo uusi sähköposti Outlookissa.
2. Valitse **Suojaa/herkkyys**  >  **-ohje ja -palaute**.
3. Valitse **Vie lokit**.
4. Tallenna lokit haluamaasi sijaintiin ja liitä ne tähän palvelupyyntöön.

Lisäresursseja:

- [Visual information protection -merkintöjen otsikon määrittäminen](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Azure Information Protection -dokumentaation tarkasteleminen](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Herkkyystarrojen käyttäminen Office-sovelluksissa](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

