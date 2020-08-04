---
title: Intune-laitteiden etähallinta TeamViewerin avulla
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554974"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>Intune-laitteiden etähallinta TeamViewerin avulla

Intunen hallitsemia laitteita voidaan hallita etänä [TeamViewerin](https://www.teamviewer.com/)avulla.

Voit hallita Intunen teamviewerin avulla seuraavasti: 

Aloita hankkimalla TeamViewerilta tunnistetiedot, joiden avulla voit määrittää TeamViewer Connectorin Intunessa. Näin järjestelmänvalvoja voi kirjoittaa tunnistetiedot TeamViewer Connector -käyttöliittymään Laitteet-kohdassa, joka on kertatoiminto Intunen ja TeamViewer-palvelun välisen yhteyden muodostamiseksi.

**Osa 1: Istunnon aloittaminen etälaitteella**

1. Valitse **Kaikki laitteet -kohdasta**laite, jolla haluat aloittaa etäistunnon.
2. Alkaen **... Lisää**, valitse **Uusi etätukiistunto**.
3. Valitse **Kyllä,** jos haluat kuitata etäistunnon.
    Kun TeamViewer-palvelu on hyväksynyt Uuden etäistunnon aloittaminen -pyynnön, näet vaihtoehdon **etätuen käynnistäminen** laitteen Yleiskuvaus-ruudun (tai Essentials)-ruudun tietojen alta. Laajenna ruutu ja näytä etätuen tila valitsemalla **Näytä lisää.**
4. Aloita istunto järjestelmänvalvojan puolella valitsemalla **Aloita etäistunto.**
5. Lataa TeamViewer-binaari (Windows) ja valitse **Suorita**.<br/>
    **Huomautus** Voit ohittaa minkä tahansa TeamViewer-web-sivustoon avatun verkkoselaimen sivun.

6. Kuittaa TeamViewer-sovelluksen pyyntö tehdä muutoksia laitteeseen (vain Windows).
7. TeamViewer-sovellus käynnistyy ja sisältää istuntokoodin yhteyden todentamiseksi etälaitteeseen.

**Osa 2: Etäistuntoon kohdistettuun laitteeseen**

1. Avaa Intune-yritysportaali.
2. Etsi ilmoitusmerkintä: "IT-järjestelmänvalvoja pyytää tämän laitteen hallintaa etätukiistuntoon" ja valitse ilmoitus.
3. Valitse TeamViewer-sovelluksen lataaminen tai TeamViewer-sovelluksen lataamisen kuittaaminen sovelluskaupasta ja valitse **Suorita**.
    **Huomautus** Voit ohittaa minkä tahansa TeamViewer-web-sivustoon avatun verkkoselaimen sivun.

4. Kuittaa TeamViewer-sovelluksen pyyntö tehdä muutoksia laitteeseen (vain Windows).
5. TeamViewer-sovellus käynnistyy ja sisältää istuntokoodin yhteyden todentamiseksi etälaitteeseen.
6. Ponnahdusikkuna kysyy, haluatko sallia istunnon aloittamisen.

**Huomautus** TeamViewer-palvelun luomat istuntokoodit ovat vain kertakäyttöiset. Jos yhteys katkeaa, sinun on

1. Sulje TeamViewer-sovelluksen esiintymä etälaitteessa ja järjestelmänvalvojan työasemassa.
2. Sulje etälaitteen yritysportaali.
3. Aloita uusi "Uusi etätukiistunto" hallintaportaalista.
4. Avaa uusi ilmoitus avaamalla etälaitteen yritysportaali uudelleen.
5. Lataa ja avaa TeamViewer-sovellus sekä etälaitteessa että järjestelmänvalvojan työasemassa, kuten ennenkin.