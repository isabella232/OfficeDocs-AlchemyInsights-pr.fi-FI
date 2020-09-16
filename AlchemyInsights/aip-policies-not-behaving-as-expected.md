---
title: 'AIP: käytännöt, joita ei voi käyttäytyä odotusten mukaan'
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
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663186"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: käytännöt, joita ei voi käyttäytyä odotusten mukaan

Azure Information Protectionin käytäntö: käytännöt, jotka eivät toimi oikein, saat ohjeita eri poliittisiin ongelmiin seuraavista ohjeista:

1. Jos sinulla on visuaalisia merkintöjä koskevia ongelmia, tarkista, [Milloin visuaalisia merkintöjä](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)käytetään.
2. Jos sinulla on automaattisia merkintöjä koskevia ongelmia, Tutustu siihen, [miten voit määrittää ehdot, jotka koskevat Azure Information Protectionin automaattista ja suositeltua luokittelua](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ja [mitä arkaluonteiset tieto tyypit](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)etsivät.
3. Jos sinulla on ongelmia Native/pfile-suojauksen kanssa, tarkista [tiedoston API-määritys](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).
4. Tarkista, käytätkö käytössä olevia käytäntöjä, joita ei ole määritetty oikein: [Azuren tietojen suojaus käytännön määrittäminen tietyille käyttäjille määritettyjen käytäntöjen avulla](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).
5. Jos automaattinen merkintä ei toimi Outlookissa, kun kiinnität merkittyä asia kirjaa, varmista, että DRMEncryptProperty-ominaisuutta ei ole määritetty tässä kuvatulla tavalla: [tieto turvan hallinnan rekisteri asetukset](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).

Jos kohtaat edelleen ongelmia, voit kerätä Azure Information Protectionin asiakas lokit ja liittää viedyt lokit tähän lipussa.

1. Avaa Office-tiedosto tai luo uusi Sähkö posti viesti Outlookissa.
2. Valitse **suojaa/herkkyys**-  >  **Ohje ja palaute**.
3. Valitse **Vie lokit**.
4. Tallenna lokit valitsemaasi sijaintiin ja liitä ne tähän palvelu pyyntöön.

Lisäresursseja:

- [Azure Information Protectionin visuaalisten merkintöjen otsikon määrittäminen](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Azure Information Protectionin ohjeiden tarkasteleminen](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Luottamuksellisuusmerkkien käyttäminen Microsoft 365-sovelluksissa](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

