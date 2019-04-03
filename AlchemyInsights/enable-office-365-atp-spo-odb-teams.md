---
title: 'ATP Office 365: n käyttöön SharePoint ja Microsoft-ryhmien OneDrive'
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2019
ms.locfileid: "31030950"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Ota käyttöön Office 365 kehittyneen uhkien suojaa SharePoint Online, OneDrive ja Microsoftin työryhmät

1. Siirry https://protection.office.com ja kirjaudu sisään.
2. Valitse **Threat management** > **käytännön** > **Turvalliset liitetiedostot**.
3. Valitse **ATP SharePoint, OneDrive-ja Microsoft-ryhmien käyttöön**, ja valitse sitten **Tallenna**.
4. (Suositus) Yleinen järjestelmänvalvoja tai SharePoint Online järjestelmänvalvojana Suorita [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet **DisallowInfectedFileDownload** -parametrin arvoksi *true*.
5. (Suositus) [Määritä hälytykset](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) havaittiin tiedostoja.

> [!NOTE]
> ATP on nJos haluat skannaus SharePoint Online OneDrive tai Microsoftin Teams kaikki yhteen tiedostoon. Tiedostot tarkistetaan asynkronisesti, prosessi, joka käyttää jakamisen ja Vieras toiminnan tapahtumat, älykäs ja uhka signaalien tunnistamiseen vahingollisia tiedostoja kautta. Katso [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).