---
title: Android-laitteiden rekisteröiminen Microsoft Intunen ongelmien vianmääritys
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759617"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Android-laitteiden rekisteröiminen Microsoft Intunen ongelmien vianmääritys

Ratkaise ongelma nyt alla olevien resurssien avulla.
  
Joitakin yleisiä kysymyksiä ja ratkaisuvaiheita:
  
 **Laite, joka ei ole salattu -virhe yritysportaalissa:** Androidin uudemmat versiot, erityisesti versiosta 7.0 alkaen, edellyttävät käynnistyskoodia varmistaaksesi, että laitteesi on täysin salattu. Yleisiä ratkaisuja ovat käynnistysnastan käyttöönotto tai laitteen salaaminen kokonaan. Lisätietoja on [tässä asiakirjassa.](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android)
  
 **Laitteet eivät voi kirjautua sisään Intune-palvelulla tai näyttää intune-hallintakonsolissa epäterveellisinä:** Jotkin Samsung 4.4- ja Samsung 5.5 -laitteet eivät välttämättä kirjaudu palveluun. Tähän ongelmaan on kolme mahdollista ratkaisua:
  
1. Avaa Intune Company Portal -sovellus manuaalisesti, joka käynnistää automaattisesti laitteen synkronoinnin.

2. Päivitä laite Android 6.0:aan tai uudempaan.

3. Poista Samsung Smart Manager käytöstä hallitsemasta Intune-yritysportaalia. Tässä [asiakirjassa](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) on lisätietoja näistä kysymyksistä ja päätöslauselmista.

 **Käyttäjäkäyttöoikeustyyppi Virheellinen** tai **Käyttäjänimi ei tunnisteta -virhe:** Käyttäjälle on määritettävä Intune- tai EMS-käyttöoikeus. Tarkista nämä asiakirjat ja määritä käyttöoikeus Office-hallintakeskuksen tai Azure-portaalin kautta.
  
Lisäresursseja ongelman ratkaisemiseen:
  
1. [Intune Troubleshooting Portalin](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) avulla voit diagnosoida ja ratkaista yleisiä rekisteröintivirheitä. Lisätietoja on [tässä asiakirjassa.](https://docs.microsoft.com/intune/help-desk-operators)

2. Tässä [asiakirjassa](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) on luettelo yleisistä virheistä, jotka estävät rekisteröitymisen ja ratkaisut kuhunkin.

3. [Lue, miten voit rekisteröidä Android-laitteet Microsoft Intuneen](https://docs.microsoft.com/intune/android-enroll).
