---
title: DataProtection – Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 3f6e48b9d2f7562d74d60c2901759a7ab359e5c67bd4aa2d556d941a41ab680c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118587"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>BitLocker-salauksen ottaminen käyttöön Intunen avulla

Intune Endpoint Protection-käytännön avulla voidaan määrittää Bitlocker-salausasetukset Windows laitteille. Lisätietoja on kohdassa Laitteiden [Windows 10 (ja uudemmat) asetukset Intunen avulla.](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)

Käytännön lisäksi Endpoint Protection on myös salausraportti, joka tarjoaa tarkemman näkymän laitteiden salauksen tilasta. Tätä raporttia voi käyttää MEM-portaalin Laitteet > **valvonta**-kohdassa ja valita sitten **Määritys-kohdassa** [Salausraportti](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport).

Jos Huomaat, että Bitlocker ei ole käytössä odotetulla tavalla tai että BitLockerin käyttöönottoon käytettävä profiili on virhetilan päällä, tutustu salausraporttiin, jotta saat paremman käsityksen siitä, miksi toiminta tapahtuu.

Lisätietoja raportin tulkitseuksesta ja eri salauksen tila-arvoista on kohdassa Laitesalauksen [valvonta Intunella.](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)

Muista, että monet uudempia laitteita, joissa Windows 10, tukevat automaattista Bitlocker-salausta, joka käynnistyy ilman mobiililaitteiden hallintakäytännön soveltamista. Tämä voi vaikuttaa käytännön sovellukseen, jos oletusasetuksia ei ole määritetty. Lisätietoja on seuraavissa usein kysytyissä kysymyksissä.

Lisätietoja BitLocker-ongelmien vianmäärityksestä on kohdassa [Microsoft Intune:n BitLocker-Microsoft Intune.](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)
 
 
**Usein kysytyt kysymykset**

K: Mitkä Windows tukevat laitesalausta käyttämällä Endpoint Protection käytäntöä?<br>
V: Intune-Endpoint Protection asetukset on otettu käyttöön [Bitlocker-CSP:n avulla.](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) Kaikki versiot tai koontiversiot eivät Windows Bitlocker-asiakastukipalvelua. <br><br>

K: Miten BitLocker voidaan ottaa käyttöön laitteissa ilman käyttäjän toimia?<br>
A: Niin kauan kuin tarvittavat edellytykset täyttyvät, Bitlocker"Silent Encryption" voidaan ottaa käyttöön Intunen kautta. Katso laitevaatimuksista ja esimerkkikäytäntöasetuksista, miten voit ottaa hiljaisen salauksen käyttöön seuraavassa tiedostossa: Silently Enable Bitlocker Encryption (Ota [Bitlocker-salaus hiljainen käyttöön).](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices) <br><br>

K: Jos laite on jo salattu BitLockerilla käyttämällä käyttöjärjestelmän salausmenetelmän ja salauksen vahvuutta (XTS-AES-128), käynnistää aseman uudelleensalauksen automaattisesti eri asetuksilla?<br>
V: Ei. Jos haluat käyttää uusia salauksen asetuksia, aseman salauksen on ensin oltava salauksen purkaminen.<br><br>
**Huomautus:** Autopilotiin rekisteröidyissä laitteissa OOBE:n aikana suoritetaan automaattinen salaus vasta, kun Intune-käytäntö on arvioitu, jolloin käytäntöpohjaisia asetuksia voidaan käyttää käyttöjärjestelmän oletusarvojen asennuksissa.
 
K: Jos laite on salattu Intune-käytännön vuoksi, poistetaanko sen salaus, kun käytäntö poistetaan?<br>
A: Salauskäytäntöjen poistaminen EI poista määritettyjen asemien salausta.
 
K: Miksi Intune-yhteensopivuuskäytäntö näyttää, että laitteeni BitLocker ei ole käytössä, vaikka se on käytössä?<br>
A: Intune-yhteensopivuuskäytännön Bitlocker käytössä -asetus hyödyntää Windows Device Health Attestation (SOVELLUKSE) -asiakasohjelmaa. Tämä asiakas mittaa vain laitteen tilan käynnistyksen yhteydessä. Jos siis laitetta ei ole käynnistetty uudelleen Bitlocker-salauksen päätyttyä, SOVELLUKSE-asiakaspalvelu ei ilmoita BitLockerista aktiiviseksi.
 
 