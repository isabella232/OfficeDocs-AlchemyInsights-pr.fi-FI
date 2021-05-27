---
title: Hyökkäyspinta-alalle vähennyssäännöt
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676230"
---
# <a name="attack-surface-reduction-rules"></a>Hyökkäyspinta-alalle vähennyssäännöt

Tiedostojen tai kansioiden poissulkeminen voi heikentää merkittävästi hyökkäyspinta-alalle vähennyssääntöjen suojausta. Tiedostot, jotka sääntö olisi estänyt, ovat sallittuja, eikä raporttia tai tapahtumaa tallenneta. Poikkeus koskee kaikkia sääntöjä, jotka sallivat poikkeukset.

ASR-poikkeukset käyttävät samaa syntaksia kuin Microsoft Defenderin virustentorjunta poissulkemiset. Lisätietoja on kohdassa [Poikkeuksien määrittäminen ja vahvistaminen Microsoft Defenderin virustentorjunta tarkistamista varten.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus) Voit välttää ongelmat tutustumaan yleisiin virheisiin, joita on [syytä välttää poissulkemista määrittäessä.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)

Kaikki ASR-säännöt eivät tue poikkeuksia. Jos haluat tarkistaa, tukeeko sääntö poikkeuksia, tutustu taulukkoon [Hyökkäyspinta-ala-vähennyssäännöt](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

## <a name="attack-surface-reduction-rules"></a>Hyökkäyspinta-alalle vähennyssäännöt

Organisaatiosi hyökkäyspinta sisältää kaikki paikat, joissa hyökkäykset voivat vaarantaa organisaation laitteita tai verkkoja. Hyökkäyspinta-alasi pienentäminen tarkoittaa organisaation laitteiden ja verkon suojaamista, jolloin hyökkäykset voidaan suorittaa vähempään eri tavalla. Hyökkäyspinta-alaan pienentämistä koskevien sääntöjen määrittäminen Microsoft Defender for Endpointissa voi auttaa.

Lisätietoja on seuraavissa artikkeleissa:

- [Yhdistä ASR-säännön GUID nimeksi](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- ASR-sääntöjen vaatimukset:
    - [Windows 10 Pro, versio 1709 tai uudempi](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise versio 1709 tai uudempi](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Palvelin, versio 1803 (puolivuosittainen kanava) tai uudempi](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Oikean poissulkemisen tunnistaminen

1. Etsi tapahtumatunnus 1121 tai 1122 Microsoft-Windows-Windows Defender/toimintalokista.

1. Arvioi lohkoskenaario ja -konteksti ja varmista, että tämän skenaarion esto on avattava.

1. Lue Tapahtuman tietojen Polku-arvo, joka on poissulkemisen määrittävä arvo.
    - Tee poissulkemisista mahdollisimman tarkkoja.
    - Käytä tarvittaessa yleismerkkiä (esimerkiksi korvaa käyttäjämuuttuja).

1. Ota poikkeus käyttöön käyttöönottotarpeiden mukaan. Lisätietoja on ohjeaiheessa [Hyökkäyspinta-alaan pienentämistä koskevien sääntöjen mukauttaminen.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)

## <a name="exclusion-is-not-honored"></a>Poissulkemista ei poisteta

1. Määritä, tukeeko sääntö poikkeuksia. Lisätietoja on kohdassa [Hyökkäyspinta-alaan pienentämistä koskevat säännöt](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).

1. Tarkista poikkeukset ja tarkista, onko tapahtumassa käytetty kirjoitusvirheitä tai väärin kirjoitettuja yleismerkkejä. Lisätietoja on kohdassa Tuetut [poikkeustyypit](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. Jos säännön vaikutus on liian suuri, harkitse säännön (takaisin) siirtäminen Valvonta-tilaan lisätarkistusta varten. Lisätietoja on kohdassa [Testaa, miten Microsoft Defender for Endpoint -ominaisuudet toimivat valvontatilassa.](/microsoft-365/security/defender-endpoint/audit-windows-defender)

1. Kerää tukitietoja tukitapauksen a avaamista varten tällä komennolla:
    
   ** MDEClientAnalyzer.cmd -v**

    Lisätietoja on kohdassa Ongelmia Microsoft [Defender for Endpointsissa onboarding-koneissa.](issues-with-onboarding-machines.md)
