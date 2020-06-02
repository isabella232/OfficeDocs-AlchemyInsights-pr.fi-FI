---
title: 305 Arkistopostilaatikon koon suurentaminen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 305
ms.assetid: ''
ms.openlocfilehash: f80b2a10ebc17cd98ed1d29b0e6ba3ca01eb1d62
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508805"
---
# <a name="increase-the-archive-mailbox-size"></a>Arkistopostilaatikon koon suurentaminen

Microsoft 365 [rajoittaa](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#mailbox-storage-limits) arkistopostilaatikoiden kokoa käyttäjätilille määritetyn käyttöoikeuden perusteella. Kun arkistopostilaatikko saavuttaa 90 % sallitusta koostaan, käyttäjä saa sähköposti-ilmoituksen. Kun arkistopostilaatikko saavuttaa kokorajoituksensa, käyttäjä ei voi siirtää enempää kohteita arkistopostilaatikkoon. Microsoft 365 ei suurenna arkistopostilaatikon kokoa, kun kokorajoitus on saavutettu. Sen sijaan käyttäjät voivat tehdä seuraavat toimet vapauttaakseen tilaa arkistopostilaatikossa:

- Vie kohteet .pst-tiedostoon Outlookin avulla.

- Poista kohteita arkistopostilaatikosta.

Microsoft 365 tarjoaa **rajoittamattoman arkistoinnin** Office 365 Enterprise E3- ja E5-käyttöoikeuksille. Järjestelmänvalvojan on otettava tämä ominaisuus käyttöön, ennen kuin arkistopostilaatikko saavuttaa enimmäiskokonsa. Kun rajoittamaton arkistointi on käytössä, voi kestää jopa 30 päivää, ennen kuin arkistopostilaatikkoon lisätään vapaata tilaa. Tämän vuoksi on suositeltavaa, että järjestelmänvalvojat tarkistavat arkistopostilaatikon vapaan tilan, jonka avulla käyttäjä voi jatkaa arkistopostilaatikon käyttöä, kun se laajenee. Lisätietoja on ohjeissa [Microsoft 365:n rajoittamattoman arkistoinnin yleiskatsaus](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving) ja [Salli rajoittamaton arkistointi Microsoft 365:ssä](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving).

Lisätietoja outlookin arkistopostilaatikon käyttämisestä on [ohjeaiheessa Outlookin vaatimukset automaattisesti laajennetun arkiston kohteiden käyttämiselle](https://docs.microsoft.com/microsoft-365/compliance/unlimited-archiving#outlook-requirements-for-accessing-items-in-an-auto-expanded-archive). Lisätietoja sellaisten säilytyskäytäntöjen määrittämisestä, jotka siirtävät kohteet automaattisesti arkistopostilaatikkoon, on [ohjeaiheessa Arkisto- ja poistokäytännön määrittäminen Microsoft 365 -organisaation postilaatikoille](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes).

**Huomautus:** Exchange 2010:n ensisijaisia postilaatikoita ei tueta automaattisesti laajeneville arkistoille.
