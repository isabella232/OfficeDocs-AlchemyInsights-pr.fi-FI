---
title: Sähkö posti viestien siirtäminen Arkisto posti laatikkoon
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799777"
---
# <a name="move-email-to-the-archive-mailbox"></a>Sähkö postin siirtäminen Arkisto posti laatikkoon

Jos haluat, että suoritat automaattiset tarkistukset alla mainittuihin asetuksiin, valitse Edellinen-painike <--sivun yläosassa ja kirjoita sitten sen käyttäjän Sähkö posti osoite, jolla on ongelmia sähkö postin siirtämiselle Arkisto posti laatikkoon.

1. Varmista, että **Arkisto posti laatikko** on otettu käyttöön. Jos näin ei ole, ota Arkisto posti laatikko käyttöön [tämän artikkelin](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) ohjeiden mukaisesti.

2. Jos haluat arkistoida viestit automaattisesti Arkisto-posti laatikkoon, **Siirrä arkistoon** -toiminnon sisältävä säilytys tunniste on määritettävä niin, että se otetaan **käyttöön automaattisesti koko posti laatikko (oletus)-tunnisteelle**. Luo tunniste seuraavasti: [Arkistoi oletus tunniste](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Lisää sitten **Arkisto** tunniste säilytys käytäntöön. Valitse Exchange-hallinta keskuksessa **säilytys käytännöt** > Lisää **Siirrä arkistoon-tunniste** käytäntöön > **Tallenna**.

4. [Liitä nyt säilytys käytännön](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) tietyn käyttäjän posti laatikkoon. Samaa käytäntöä sovelletaan sekä **perus** -että **Arkisto** posti laatikkoon.

On ehkä tarpeen pakottaa hallitun kansion avustaja (MFA) suorittamaan uudet asetukset käyttäjän posti laatikkoon ja käyttämään niitä. Suorita seuraava komento, kun olet [muodostanut yhteyden EXO PowerShelliin](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) tietyn posti laatikon hallittujen kansioiden hallinnan aloittamiseksi:
  
Käynnistä-Managedfoldadassistant-Identity <name of the mailbox>

Lisä tietoja arkistointi käytäntöjen määrittämisestä on kohdassa [Arkisto-ja poisto käytäntöjen määrittäminen Posti laatikoille](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  