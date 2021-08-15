---
title: Automaattinen luokitus ei toimi odotetulla tavalla AIP-asiakasohjelmassa
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
- "4373"
ms.openlocfilehash: 93d15b8b65fd52a567ecbb6e1f84363bf2b38946c105896b0b5ef41e49d16ea9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53979706"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automaattinen luokitus ei toimi odotetulla tavalla AIP-asiakasohjelmassa

Automaattinen luokitus ei toimi odotetulla tavalla. Tutustu seuraaviin suositeltuihin ohjeisiin:

1. Jos automaattisen merkitsemisen kanssa on ongelmia, tutustu kohtiin [Azure Information Protectionin automaattisen ja suositellun luokituksen ehtojen määrittäminen](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ja [Mitä luottamukselliset tietolajit etsivät](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Tarkista, käytätkö kohdistettuja käytäntöjä, joita ei ole määritetty oikein: [Azure Information Protection -käytännön määrittäminen tietyille käyttäjille kohdistettujen käytäntöjen avulla](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Jos automaattinen luokitus ei toimi Outlookissa, kun merkittyä asiakirjaa liitetään, varmista, ettei kohdetta `DRMEncryptProperty` ole määritetty täällä avatulla tavalla: [Suojauksen IRM-rekisteriasetukset](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Jos käytit Azure Information Protection -käytännössä [valmiita tietolajeja](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b), varmista, että sisältö vastaa odotettua muotoa.
5. Varmista, että merkinnäksi on määritetty oikein **Automaattinen** tai **Suositeltu**. (**Automaattinen**-merkintä on käytettävissä kaikissa Microsoft 365 -sovelluksissa, kun taas **Suositeltu** on käytettävissä kaikissa Microsoft 365 -sovelluksissa Outlookia lukuun ottamatta.)
6. Et voi käyttää automaattista luokitusta tiedostoissa ja sähköposteissa, jotka on luokiteltu aiemmin manuaalisesti tai luokiteltu aiemmin manuaalisesti korkeampaan luokitukseen.  Lisätietoja on kohdassa [Automaattisten tai suositeltujen selitteiden lisääminen](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Jos ongelmia ilmenee edelleen, kerää Azure Information Protection -asiakaslokit ja liitä viedyt lokit tukipyyntöön. Azure Information Protection -lokien vieminen:
    - Avaa Office-tiedosto tai luo uusi sähköpostiviesti Outlookissa.
    - Valitse **Suojaus ja luottamuksellisuus** > **Ohje- ja palaute**.
    - Valitse **Vie lokit**.
    - Tallenna lokit haluamaasi sijaintiin ja liitä ne palvelupyyntöösi.

Katso lisätietoja seuraavista:

- [Azure Information Protectionin automaattisen ja suositellun luokituksen ehtojen määrittäminen](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Ohjeita yleisiin skenaarioihin, joissa käytetään Azure Information Protectionia](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Tutustu Azure Information Protection -ohjeisiin](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Azure Information Protection -tilausten ja -ominaisuuksien tarkistaminen](https://azure.microsoft.com/pricing/details/information-protection)
- [Azure Information Protectionin vaatimukset](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Azure Information Protectionin pika-aloitusopas](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Lataa Azure Information Protection -asiakasohjelma](https://www.microsoft.com/download/details.aspx?id=53018)
