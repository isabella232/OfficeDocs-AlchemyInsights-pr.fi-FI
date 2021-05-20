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
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543925"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Ota Käyttöön Microsoft Defender for Office 365 for SharePoint Online, OneDrive ja Microsoft Teams

1. Siirry ja https://protection.office.com kirjaudu sisään.
2. Valitse **Uhkien**  >  **hallintakäytännön**  >  **turvalliset liitteet**.
3. Valitse **Turn on Defender for Office 365 for SharePoint, OneDrive and Microsoft Teams** ja valitse sitten **Tallenna**.
4. (Suositus) Suorita yleisenä järjestelmänvalvojana tai SharePoint Online [-järjestelmänvalvojana Set-SPOTenant-cmdlet-komento,](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) kun **DisallowInfectedFileDownload-parametrin** arvoksi on määritetty *tosi*.
5. (Suositus) [Määritä havaittujen](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) tiedostojen ilmoitukset.

> [!NOTE]
> Microsoft Defender for Office 365 ei tarkista jokaista yksittäistä tiedostoa SharePoint Onlinessa, OneDrive tai Microsoft Teams. Tiedostot tarkistetaan asynkronisesti jakamis- ja vierastoimintatapahtumia käyttävän prosessin sekä älykkäiden heurististen ja uhkien signaaleiden avulla haittaohjelmien tunnistamiseen. Katso [Microsoft Defender for Office 365 for SharePoint, OneDrive ja Microsoft Teams.](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)