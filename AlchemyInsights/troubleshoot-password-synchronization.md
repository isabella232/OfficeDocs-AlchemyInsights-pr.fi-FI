---
title: Salasanasynkronoinnin vianmääritys
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105746"
---
# <a name="troubleshoot-password-synchronization"></a>Salasanasynkronoinnin vianmääritys

Aloita salasanojen synkronointiongelmien vianmääritys käyttämällä tätä AAD Näyttöyhteys vianmääritystehtävää sen selvittämiseksi, miksi salasanat eivät synkronoidu. Aloita valitsemalla Suoran [synkronoinnin hallinta.](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)  

1. Avaa uusi Windows PowerShell Azure AD Näyttöyhteys -palvelimessa ja valitse **Suorita järjestelmänvalvojana -vaihtoehto.**

2. Suorita Set-ExecutionPolicy RemoteSigned tai Set-ExecutionPolicy Unrestricted.

3. Käynnistä ohjattu Azure AD Näyttöyhteys toiminto.

4. Siirry Lisätehtävät-sivulle > **Vianmääritys**  >  **Seuraava.**

5. Avaa  PowerShellin vianmääritysvalikko valitsemalla Käynnistä.

6. Valitse **Salasanasynkronoinnin vianmääritys.**

    Ongelma johtuu yleensä siitä, että tietyn käyttäjätilin salasanaa ei synkronoida.

    **Huomautukset** Salasanasynkronointi epäonnistuu, jos viimeisin onnistunut salasanasynkronointi oli jokin aika sitten.

Lisätietoja salasanojen synkronoinnin vianmäärityksestä on ohjeaiheessa [Salasanojen hash-synkronoinnin vianmääritys Azure AD Näyttöyhteys synkronoinnin kanssa.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)