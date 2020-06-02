---
title: Office 365 ATP:n ottaminen käyttöön SharePointissa, OneDrivessa ja Microsoft Teamsissa
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506915"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Office 365:n Advanced Threat Protectionin ottaminen käyttöön SharePoint Onlinessa, OneDrivessa ja Microsoft Teamsissa

1. Mene https://protection.office.com sisään ja kirjaudu sisään.
2. Valitse **Uhkien**  >  **hallintakäytännön**  >  **turvalliset liitteet**.
3. Valitse **Ota ATP käyttöön SharePointissa, OneDrivessa ja Microsoft Teamsissa**ja valitse sitten **Tallenna**.
4. (Suositus) Suorita [Set-SPOTenant-cmdlet-komento](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) yleisenä järjestelmänvalvojana tai SharePoint Online -järjestelmänvalvojana siten, että **DisallowInfectedFileDownload-parametrin** arvo on *true*.
5. (Suositus) [Määritä havaittujen tiedostojen hälytykset.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files)

> [!NOTE]
> ATP tarkistaa jokaisen tiedoston SharePoint Onlinessa, OneDrivessa tai Microsoft Teamsissa. Tiedostot skannataan asynkronisesti jakamis- ja vierastoimintatapahtumia käyttävän prosessin kautta sekä älykkäiden heuristiikka- ja uhkasignaalien avulla haitallisten tiedostojen tunnistamiseen. Katso [SHAREPointin, OneDriven ja Microsoft Teamsin ATP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)