---
title: Käyttäjäkuva näkyy edelleen Microsoft Teams organisaatiokaaviossa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422211"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Käyttäjäkuva näkyy edelleen Microsoft Teams organisaatiokaaviossa

Jos yksi tai useampi organisaatiosi käyttäjä on poistettu käytöstä tai poistettu ja profiilikuva näkyy edelleen organisaatiokaaviossa, **on** mahdollista, että NäytäOsoiteluettelot-asetuksena on Epätosi: 

1. Siirry Microsoft 365 -hallintakeskus > [aktiivisten käyttäjien](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) käyttäjiin ja valitse käyttäjä, jolla on edelleen näkyvissä oleva valokuva. 
1. Valitse **Sähköposti-välilehti** ja varmista, että **Näytä yleisessä osoiteluettelossa -asetuksena** on **Ei**.

Jos **ShowInAddressLists-asetuksen** arvoksi ei ole määritetty Ei, tarkista seuraavat asiat:  

- Käyttäjä saattaa olla näkyvissä vastaanottajaluettelosta Exchange. Lisätietoja on artikkelissa [Osoiteluetteloiden hallinta Exchange Online.](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists) 
- Käyttäjä saattaa olla näkyvissä osoiteluettelosta Azure Active Directory. Lisätietoja on kohdassa [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 