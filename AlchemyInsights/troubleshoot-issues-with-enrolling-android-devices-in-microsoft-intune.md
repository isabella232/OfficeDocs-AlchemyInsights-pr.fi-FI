---
title: Android-laitteiden rekisteröintiongelmien vianmääritys Microsoft Intunessa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708995"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Android-laitteiden rekisteröintiongelmien vianmääritys Microsoft Intunessa

Ratkaise ongelmasi nyt alla lueteltujen resurssien avulla.
  
Joitakin yleisiä ongelmia ja ratkaisuvaiheita:
  
 **Laite ei ole salattu -virhe yritysportaalissa:** Androidin uudempien versioiden, erityisesti v7.0-version, on oltava käynnistyksen tunnuskoodi, jotta varmistat, että laitteesi on täysin salattu. Yleisiä ratkaisuja ovat käynnistystallenuksen ottaminen käyttöön tai laitteen täysin salaaminen. Katso [lisätietoja tästä](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) asiakirjasta.
  
 **Laitteet eivät pysty sisään Intune-palvelussa tai näkyvät epäterveellisenä Intune-hallintakonsolissa:** Jotkin Samsung 4.4- ja 5.5-laitteet eivät välttämättä tarkista palvelua. Tähän ongelmaan on kolme mahdollista ratkaisua:
  
1. Avaa Manuaalisesti Intune-yritysportaalisovellus, joka aloittaa laitteen synkronoinnin automaattisesti.

2. Päivitä laite Android 6.0-versioon tai sitä uudempiin versioihin.

3. Poista Samsung Smart Manager käytöstä hallitsemalla Intune-yritysportaalia. Tässä [asiakirjassa on](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) lisätietoja näistä ongelmista ja ratkaisuista.

 **Käyttäjäkäyttöoikeustyyppi** **virheellinen tai käyttäjänimiä** ei tunnisteta -virhe: Käyttäjälle on oltava määritetty Intune- tai EMS-käyttöoikeus. Tarkista nämä tiedostot ja määritä käyttöoikeus Office-hallintakeskuksen tai Azure-portaalin kautta.
  
Lisäresursseja ongelman ratkaisemiseen:
  
1. [Intunen vianmääritysportaalin avulla](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) voit diagnosoida ja ratkaista yleisiä rekisteröintivirheitä. Katso [lisätietoja tästä](https://docs.microsoft.com/intune/help-desk-operators) asiakirjasta.

2. Tässä [asiakirjassa on](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) luettelo yleisistä virheistä, jotka estävät kunkin rekisteröinnin ja ratkaisut.

3. [Opi rekisteröimaan Android-laitteet Microsoft Intunessa.](https://docs.microsoft.com/intune/android-enroll)
