---
title: Sala sanan synkronoinnin vian määritys
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
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664923"
---
# <a name="troubleshoot-password-synchronization"></a>Sala sanan synkronoinnin vian määritys

Voit määrittää Sala sanojen synkronointi ongelmien vian määrityksen käynnistämällä tämän AAD Connect-vian määritys tehtävän avulla, miksi Sala sanat eivät synkronoidu. Aloita siirtymällä kohtaan [suoran synkronoinnin hallinta](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Avaa uusi Windows PowerShell-istunto Azure AD Connect-palvelimessa ja valitse **Suorita järjestelmänvalvojana** -vaihto ehto.

2. Suorita sarja-ExecutionPolicy Remotsigned-tai ExecutionPolicy-käytäntönsä rajoittamattomat.

3. Käynnistä ohjattu Azure AD Connect-toiminto.

4. Siirry lisä tehtävät-sivulle > **vian määritys**  >  **Seuraava**.

5. Avaa PowerShellin vian määritys-valikko valitsemalla **Käynnistä** .

6. Valitse **Sala sanan synkronoinnin vian määritys**.

    Ongelma on yleensä se, että tietyn käyttäjä tilin Sala sanaa ei synkronoida.

    **Huomautukset** Sala sanojen synkronointi epäonnistuu, jos viimeinen onnistunut sala sana synkronoidaan jonkin aikaa sitten.

Lisä tietoja Sala sanan synkronoinnin vian määrityksestä on Ohje aiheessa [Sala sanan hajautus synkronoinnin vian määritys Azure AD Connect-synkronoinnin avulla](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).