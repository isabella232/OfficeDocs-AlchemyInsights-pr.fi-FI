---
title: Android-laitteiden rekisteröintiongelmien vianmääritys Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 0ae926e6b31493e7359981c621fd27e8f53d49a17bdf107173b087fe6cc688fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54008075"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Android-laitteiden rekisteröintiongelmien vianmääritys Microsoft Intune

Ratkaise ongelma nyt alla lueteltujen resurssien avulla.
  
Joitakin yleisiä ongelmia ja ratkaisuvaiheita:
  
 **Laite ei ole salattu -virhe Yritysportaali:** Androidin uudempi versio, erityisesti v7.0-versiosta alkaen, edellyttää käynnistyksen tunnuskoodia, jotta voit varmistaa, että laitteesi on täysin salattu. Yleisiä ratkaisuja ovat käynnistyksen PIN-koodin ottaminen käyttöön tai laitteen täysin salaaminen. Katso [lisätietoja](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) tästä asiakirjasta.
  
 Laitteet eivät pysty tarkistamaan intune-palvelua tai näy huonolla hetkellä **Intune-hallintakonsolissa:** Jotkin Samsung 4.4- ja 5.5-laitteet eivät välttämättä tarkista palvelua. Tähän ongelmaan on kolme mahdollista ratkaisua:
  
1. Voit avata Intune-yritysportaali, joka aloittaa laitteen synkronoinnin automaattisesti.

2. Päivitä laitteeseen Android 6.0 tai uudempi.

3. Poista Samsung Smart Managerin hallinta käytöstä Intune-yritysportaali. Tässä [asiakirjassa on](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) lisätietoja näistä ongelmista ja ratkaisuista.

 **Käyttäjän käyttöoikeustyyppi Virheellinen** **tai Käyttäjänimi ei** tunnistettu -virhe: Käyttäjälle on oltava määritetty Intune- tai EMS-käyttöoikeus. Tarkista nämä asiakirjat ja määritä käyttöoikeus Office hallintakeskuksen tai Azure-portaalin kautta.
  
Lisäresursseja ongelman ratkaisemiseksi:
  
1. [Intunen vianmääritysportaalin avulla voit](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) tehdä vianmäärityksen ja ratkaista yleisiä rekisteröintivirheitä. Katso [lisätietoja](https://docs.microsoft.com/intune/help-desk-operators) tästä asiakirjasta.

2. Tarkista [tästä asiakirjasta](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) luettelo yleisistä virheistä, jotka estävät jokaisen rekisteröinnin ja ratkaisut.

3. [Opi rekisteröimaan Android-laitteet Microsoft Intune.](https://docs.microsoft.com/intune/android-enroll)
