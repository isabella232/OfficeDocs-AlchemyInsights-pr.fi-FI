---
title: 1374 kahden posti laatikon HOWTO-ongelman ratkaiseminen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1374"
- "2692"
- "3500014"
ms.assetid: 8bf1a8f2-58ef-4697-b9c0-be340de96bfe
ms.openlocfilehash: 048c527b26d138535550b5bae399d0ce9fbce0a6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720895"
---
# <a name="a-user-has-two-mailboxes"></a>Käyttäjällä on kaksi posti laatikkoa

Azure Active Directory Connect (AAD Connect)-tai DirSync-sovelluksessa käytettävät yhdistelmä ympäristöt saattavat vahingossa aiheuttaa käyttäjälle kaksi posti laatikkoa: yhden paikallisen ja yhden pilvi palvelussa. Päällekkäinen posti laatikko voidaan luoda kummassakin paikassa.

Jos haluat korjata ongelman, Lue [ohjeet siihen, miten voit palauttaa, kun posti laatikko on olemassa sekä Exchange Onlinessa että paikallisessa sijainnissa](https://docs.microsoft.com/exchange/troubleshoot/move-mailboxes/mailbox-exists-exo-onpremises). Jos haluat lisä tietoja siitä, miten voit välttää tämän jatkossa, Katso, onko [käyttäjäni posti laatikko sekä paikallinen että Exchange Onlinessa. Apua!](https://techcommunity.microsoft.com/t5/Exchange-Team-Blog/My-user-has-a-mailbox-both-on-premises-and-in-Exchange-Online/ba-p/846809).
