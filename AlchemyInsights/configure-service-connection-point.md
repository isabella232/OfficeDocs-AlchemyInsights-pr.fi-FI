---
title: Palveluyhteyspisteen (SCP) määrittäminen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035452"
---
# <a name="configure-service-connection-point-scp"></a>Palvelun yhteyspisteen (SCP) määrittäminen

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Syy:** SCP-objektin lukeminen ja Azure AD -vuokraajan tietojen saaminen ei onnistu
- **Ratkaisu:** Katso kohta [Palveluyhteyspisteen määrittäminen](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Toimintasuunnitelma**

- Tarkista, onko laite saanut GPO:n hallittua vahvistusta varten.
- Varmista, että GPO on luonut rekisteriavaimet.
- Varmista, että sinulla on kaksi avainta, jotka on luotu hakemistotunnuksella ja onmicrosoft-toimialueella.

**Asiakaspuolen rekisteriasetuksen määrittäminen SCP:lle**

Seuraavan esimerkin avulla voit luoda ryhmäkäytäntöobjektin ottaaksesi käyttöön rekisteriasetuksen, joka määrittää SCP-merkinnän laitteiden rekisterissä.

1. Avaa ryhmäkäytäntöjen hallintakonsoli ja luo uusi ryhmäkäytäntöobjekti toimialueellesi.
     - Anna juuri luomallesi GPO:lle nimi (esimerkiksi ClientSideSCP)

2. Muokkaa käyttäjäkäytäntöobjektia ja etsi seuraava polku: tietokoneen > asetukset > Windowsin > **rekisteriin.**

3. Napsauta Rekisteri-kohtaa **hiiren kakkospainikkeella** **ja valitse > rekisterikohde.**

4. Määritä **Yleiset-välilehdessä** seuraavat asetukset:
  
- **Toiminto:** Päivitä
    
- **Rakenne :** HKEY_LOCAL_MACHINE
    
- **Avainpolku:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Arvon nimi**: Vuokraajatunnus
    
- **Arvotyyppi:** REG_SZ
    
- **Arvotiedot:** Azure AD -esiintymän GUID- tai hakemistotunnus (tämä arvo > **Azure Active Directory ->-ominaisuuksien > hakemistotunnuksesta)**
 
- Valitse **OK**.
 
5. Napsauta Rekisteri-kohtaa **hiiren kakkospainikkeella** **ja valitse > rekisterikohde.**

6. Määritä **Yleiset-välilehdessä** seuraavat asetukset:
  
- **Toiminto:** Päivitä
    
- **Rakenne :** HKEY_LOCAL_MACHINE
    
- **Avainpolku:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Arvon nimi**: VuokraajanNimi
    
- **Arvotyyppi:** REG_SZ
    
- **Arvon tiedot:** Varmennettu toimialuenimesi, jos käytät liitettyä ympäristöä, kuten AD FS:ää. Varmennettu toimialuenimi tai onmicrosoft.com toimialuenimi (esimerkiksi contoso.onmicrosoft).com, jos käytät hallittua ympäristöä

- Valitse **OK**.

7. Sulje juuri luodun GPO:n editori.

8. Linkitä juuri luotu GPO haluttuun OU:han, joka sisältää toimialueeseen liitettyja tietokoneita, jotka kuuluvat valvotulle koontipopulaatiolle.

Lisätietoja on kohdassa [Azure AD -yhdistelmäympäristön liitoksen hallittu vahvistus – Azure AD | Microsoft Docs ja](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) [Azure Active Directoryyn liitettyjen yhdistelmälaitteiden | Microsoft Docs.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current)









