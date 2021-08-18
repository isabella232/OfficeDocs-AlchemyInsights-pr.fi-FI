---
title: ATP Office 365 käyttöön SharePoint, OneDrive ja Microsoft Teams
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
ms.openlocfilehash: 2d132101768e0a835d448604d684ec0c735e6628
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332156"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Ota Käyttöön Microsoft Defender for Office 365 for SharePoint Online, OneDrive ja Microsoft Teams

1. Siirry ja https://protection.office.com kirjaudu sisään.
2. Valitse **Uhkien**  >    >  **hallintakäytäntö Lokero liitteet.**
3. Valitse **Ota Defender for Office 365 käyttöön SharePoint OneDrive** ja Microsoft Teams ja valitse sitten **Tallenna**.
4. (Suositus) Suorita yleisenä järjestelmänvalvojana tai SharePoint Online -järjestelmänvalvojana [Set-SPOTenant-cmdlet-komento](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) ja määritä **DisallowInfectedFileDownload-parametrin** arvoksi *tosi*.
5. (Suositus) [Määritä havaittujen](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) tiedostojen ilmoitukset.

**Huomautus:** Microsoft Defender for Office 365 ei tarkista jokaista SharePoint Onlinessa, OneDrive tai Microsoft Teams. Tiedostot tarkistetaan asynkronisesti jakamis- ja vierastoimintatapahtumia käyttävän prosessin sekä älykkäiden heurististen ja uhkien signaaleiden avulla haittaohjelmien tunnistamiseen. Katso [Microsoft Defender for Office 365 SharePoint, OneDrive ja Microsoft Teams.](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)
