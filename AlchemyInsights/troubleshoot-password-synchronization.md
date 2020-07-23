---
title: Salasanan synkronointiin liittyviä ongelmia
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387874"
---
# <a name="troubleshoot-password-synchronization"></a>Salasanan synkronointiin liittyviä ongelmia

Voit tehdä salasanojen synkronointiongelmien vianmäärityksen käynnistämällä tämän AAD Connect -vianmääritystehtävän avulla, miksi salasanoja ei synkronoida. Aloita siirtymällä [kohtaan Suoran synkronoinnin hallinta](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Avaa uusi Windows PowerShell -istunto Azure AD Connect -palvelimessa ja valitse **Suorita järjestelmänvalvojana** -vaihtoehto.

2. Suorita Set-ExecutionPolicy RemoteSigned tai Set-ExecutionPolicy Unrestricted.

3. Käynnistä ohjattu Azure AD Connect -toiminto.

4. Siirry Lisätehtävät-sivulle > **Seuraava - vianmääritys**  >  **Next**.

5. Avaa PowerShellin vianmääritysvalikko valitsemalla **Käynnistä.**

6. Valitse **Salasanan synkronoinnin vianmääritys**.

    Ongelmana on yleensä se, että salasanaa ei synkronoida tietylle käyttäjätilille.

    **Osan sisällöstä toimittaa** Salasanan synkronointi epäonnistuu, jos viimeinen onnistunut salasanan synkronointi oli jokin aika sitten.

Lisätietoja salasanojen synkronoinnin vianmäärityksestä on [ohjeaiheessa Salasanan hajautussynkronoinnin vianmääritys Azure AD Connect -synkronoinnin kanssa](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).