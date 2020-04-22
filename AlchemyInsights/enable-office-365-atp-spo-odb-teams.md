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
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703423"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Office 365 Advanced Threat Protectionin ottaminen käyttöön SharePoint Onlinessa, OneDrivessa ja Microsoft Teamsissa

1. Mene https://protection.office.com sisään ja kirjaudu sisään.
2. Valitse **Uhkien** > **hallintakäytännön** > **turvalliset liitteet**.
3. Valitse **Ota ATP sharepointiin, OneDriveen ja Microsoft Teamsiin käyttöön**ja valitse sitten **Tallenna**.
4. (Suositus) Yleisenä järjestelmänvalvojana tai SharePoint Online -järjestelmänvalvojana suorita [Set-SPOTenant-cmdlet-tiedosto,](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) jonka **DisallowInfectedFileDownload-parametrin** arvo on *true*.
5. (Suositus) [Määritä havaittujen tiedostojen hälytykset.](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files)

> [!NOTE]
> ATP tarkistaa jokaisen tiedoston SharePoint Onlinessa, OneDrivessa tai Microsoft Teamsissa. Tiedostot skannataan asynkronisesti prosessilla, joka käyttää jakamista ja asiakkaiden toimintatapahtumia sekä älykkäitä heuristiikkaa ja uhkasignaaleja haitallisten tiedostojen tunnistamiseen. Katso [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).