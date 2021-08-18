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
ms.openlocfilehash: 4a29fdf1b61dd51b85793a1346bea193c67f70d32344470cb5449cf767da4a24
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896600"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Ota Käyttöön Microsoft Defender for Office 365 for SharePoint Online, OneDrive ja Microsoft Teams

1. Siirry ja https://protection.office.com kirjaudu sisään.
2. Valitse **Uhkien**  >    >  **hallintakäytäntö Lokero liitteet.**
3. Valitse **Turn on Defender for Office 365 for SharePoint, OneDrive and Microsoft Teams** ja valitse sitten **Tallenna**.
4. (Suositus) Suorita yleisenä järjestelmänvalvojana tai SharePoint Online [-järjestelmänvalvojana Set-SPOTenant-cmdlet-komento,](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) jossa **DisallowInfectedFileDownload-parametrin** arvoksi on määritetty *tosi.*
5. (Suositus) [Määritä havaittujen](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) tiedostojen ilmoitukset.

> [!NOTE]
> Microsoft Defender for Office 365 ei tarkista jokaista SharePoint Onlinessa, OneDrive tai Microsoft Teams. Tiedostot tarkistetaan asynkronisesti jakamis- ja vierastoimintatapahtumia käyttävän prosessin sekä älykkäiden heurististen ja uhkien signaaleiden avulla haittaohjelmien tunnistamiseen. Katso [Microsoft Defender for Office 365 SharePoint, OneDrive ja Microsoft Teams.](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)