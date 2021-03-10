---
title: Windows 10 -laitteiden määrittäminen Microsoft Intunen perusaikataulujen avulla
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50694430"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Microsoft Intune -suojauksen perusaikataulujen käyttäminen Windows 10 -laitteiden määrittämiseen

Intune-suojauksen perusaikataulut auttavat suojaamaan käyttäjiä ja laitteita. Suojauksen perusaikataulut ovat Windowsin asetusten ennalta määritettyjä ryhmiä, joiden avulla käytetään tunnettua asetus- ja oletusarvoryhmää, jota asianomaiset suojausryhmät suosittelevat. Luomalla suojauksen perusaikataulun profiilin Intunessa luot mallin, joka koostuu useista laitemääritysprofiileista.

Kun otat suojauksen perusaikataulut käyttöön käyttäjä- tai laiteryhmissä, asetukset otetaan käyttöön laitteissa, jotka suoritetaan Windows 10:ssä tai sitä uudemmassa versiossa. Esimerkiksi Microsoft mobile device management (MDM) -suojauksen perusaikataulu (1) ottaa BitLockerin käyttöön siirrettäville asemille (2) edellyttää salasanan laitteen lukituksen avaamista varten ja (3) poistaa perustodennuksen käytöstä. Jos oletusarvo ei toimi ympäristössäsi, voit mukauttaa perusaikataulua haluamallasi asetuksilla.

Suojauksen perusaikataulut auttavat myös muodostamaan lopusta päähän -suojatun työnkulun Microsoft 365:ssä. Seuraavassa on joitakin tämän toiminnon etuja:
- Suojauksen perusaikataulu sisältää parhaat käytännöt ja suositukset tietoturvaan vaikuttavia asetuksia varten. Koska Intune-kumppanit Windowsin suojaustiimin kanssa luovat perusaikatauluja ryhmäkäytäntöjä varten, nämä suositukset perustuvat vankkaihin ohjeisiin ja laajaan käyttökokemukseen.
- Jos et ole ennen luonut Intunea etkä ole varma, mistä aloittaa, suojauksen perusaikataulujen avulla voit luoda ja ottaa käyttöön suojatun profiilin nopeasti.
- Jos käytät tällä hetkellä ryhmäkäytäntöä, siirtyminen Intuneen hallintaa varten on huomattavasti helpompaa suojauksen perusaikataulujen avulla, koska nämä suojauksen perusaikataulut sisältyvät Intuneen ja sisältävät hallinnan huippuominaisuuksia.

Lisätietoja on ohjeaiheessa Windowsin suojauksen [perusaikataulut ja](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) [mobiililaitteiden hallinta.](https://docs.microsoft.com/windows/client-management/mdm/)