---
title: Käyttäjäkuva ei näy Microsoft Teams organisaatiokaaviossa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792693"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Käyttäjäkuva ei näy Microsoft Teams organisaatiokaaviossa

Jos vähintään yksi organisaatiosi käyttäjä puuttuu profiilikuvastaan organisaatiokaaviossa, on mahdollista, että **Asetuksen ShowInAddressLists** arvoksi on määritetty **Epätosi:**

1. Siirry Microsoft 365 -hallintakeskus > [**aktiivisten käyttäjien käyttäjiin**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)ja valitse käyttäjä, jolla puuttuva kuva on. 
1. Valitse **Sähköposti-välilehti** ja varmista, että **Näytä yleisessä osoiteluettelossa -asetuksena** on **Kyllä**. 

Jos **ShowInAddressLists-asetuksen** asettaminen Kyllä-arvoksi ei toimi, tarkista seuraavat asiat: 

- Käyttäjä on ehkä piilotettu vastaanottajaluettelosta Exchange. Lisätietoja on artikkelissa [Osoiteluetteloiden hallinta Exchange Online.](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists) 
- Käyttäjä on ehkä piilotettu osoiteluettelosta Azure Active Directory. Lisätietoja on kohdassa [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 
