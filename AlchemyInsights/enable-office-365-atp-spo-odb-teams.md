---
title: ATP Office 365 n käyttöönotto SharePoint, OneDrive ja Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 61ca448ef146f3f6fb930f0dc6f09f41bde72087f56ffba820f0a2d517cddb31
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53964630"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Ota Käyttöön Microsoft Defender for Office 365 for SharePoint Online, OneDrive ja Microsoft Teams

1. Siirry ja https://protection.office.com kirjaudu sisään.
2. Valitse **Uhkien**  >    >  **hallintakäytäntö Lokero liitteet.**
3. Valitse **Turn on Defender for Office 365 for SharePoint, OneDrive and Microsoft Teams** ja valitse sitten **Tallenna**.
4. (Suositus) Suorita yleisenä järjestelmänvalvojana tai SharePoint Online [-järjestelmänvalvojana Set-SPOTenant-cmdlet-komento,](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) kun **DisallowInfectedFileDownload-parametrin** arvoksi on määritetty *tosi*.
5. (Suositus) [Määritä havaittujen](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) tiedostojen ilmoitukset.

> [!NOTE]
> Microsoft Defender for Office 365 ei tarkista jokaista yksittäistä tiedostoa SharePoint Onlinessa, OneDrive tai Microsoft Teams. Tiedostot tarkistetaan asynkronisesti jakamis- ja vierastoimintatapahtumia käyttävän prosessin sekä älykkäiden heurististen ja uhkien signaaleiden avulla haittaohjelmien tunnistamiseen. Katso [Microsoft Defender for Office 365 for SharePoint, OneDrive ja Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)