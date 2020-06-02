---
title: Automaattinen luokittelu ei toimi odotetulla tavalla AIP-asiakkaan kanssa
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
- "4373"
ms.openlocfilehash: 22eeb6ba32e4e943efa2495a477ff394f3c135db
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508373"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>Automaattinen luokittelu ei toimi odotetulla tavalla AIP-asiakkaan kanssa

Automaattinen luokitus ei toimi odotetulla tavalla, käytä seuraavia suositeltuja ohjeita:

1. Jos automaattisessa merkintöjen yhteydessä on ongelmia, katso [Lisätietoja on ohjeaiheessa Azure Information Protectionin automaattisen ja suositellun luokituksen ehtojen määrittäminen](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ja [arkaluonteisten tietotyyppien etsiminen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).
2. Tarkista, käytätkö vaikutusaluekäytäntöjä, joita ei ole määritetty oikein: [Azure Information Protection -käytännön määrittäminen tietyille käyttäjille vaikutusaluekäytäntöjen avulla](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
3. Jos automaattinen merkintä ei toimi Outlookissa, kun liität merkittyä asiakirjaa, varmista, että sitä `DRMEncryptProperty` ei ole määritetty tässä kuvatulla tavalla: [IRM-rekisteriasetukset suojausta varten](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).
4. Jos käytit Azure Information Protection -käytännön [valmiita tietotyyppejä,](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) varmista, että sisältösi vastaa odotettua muotoa.
5. Varmista, että otsikko on määritetty oikein **automaattista** tai **suositeltua**varten. **(Automaattinen** merkintä on käytettävissä kaikissa Office-sovelluksissa, kun taas **Suositeltava** on käytettävissä kaikissa Office-sovelluksissa Outlookia lukuun ottamatta.)
6. Automaattista luokittelua ei voi käyttää asiakirjoissa ja sähköposteissa, jotka on aiemmin merkitty manuaalisesti tai jotka on aiemmin merkitty automaattisesti korkeammalla luokituksella.  Lisätietoja on kohdassa [Automaattisten tai suositeltujen tarrojen käyttäminen](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).
7. Jos ongelmat jatkuvat, kerää Azure Information Protection -asiakaslokit ja liitä viedyt lokit tukilippuusi. Azure Information Protection -lokien vieminen:
    - Avaa Office-asiakirja tai luo uusi sähköposti Outlookissa.
    - Valitse **Suojaa/herkkyys**  >  **-ohje ja -palaute**.
    - Valitse **Vie lokit**.
    - Tallenna lokit haluamaasi sijaintiin ja liitä ne palvelupyyntöysi.

Lisätietoja on seuraavissa ohjeissa:

- [Azure Information Protectionin automaattisen ja suositellun luokituksen ehtojen määrittäminen](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Azure Information Protection -suojausta käyttävien yleisten skenaarioiden toimintaohjeet](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Azure Information Protection -dokumentaation tarkasteleminen](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Azure Information Protection -tilausten ja -ominaisuuksien tarkasteleminen](https://azure.microsoft.com/pricing/details/information-protection)
- [Azure-tietojen suojausta koskevat vaatimukset](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Azure Information Protectionin pika-aloitusopas](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Lataa Azure Information Protection -asiakasohjelma](https://www.microsoft.com/download/details.aspx?id=53018)
