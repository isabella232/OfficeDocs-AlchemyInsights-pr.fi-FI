---
title: Office 365 ATP:N käyttöönottaminen SharePointissa, OneDrivessa ja Microsoft Teamsissa
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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709904"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Office 365 Advanced Threat Protectionin käyttöönotto SharePoint Onlinessa, OneDrivessa ja Microsoft Teamsissa

1. Siirry kohtaan https://protection.office.com ja Kirjaudu sisään.
2. Valitse **uhkien hallinta**  >  **käytännön**  >  **turvalliset liitteet**.
3. Valitse **Ota SharePoint-, OneDrive-ja Microsoft TEAMSIN ATP käyttöön**ja valitse sitten **Tallenna**.
4. Suositellut Jos sinulla on yleinen järjestelmänvalvojana tai SharePoint Online-järjestelmänvalvojana, suorita [-spoalion cmdlet-](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) komentosovelma, jonka **Disallowinfectedfiledownload** -parametrin arvona on *True*.
5. Suositellut [Määritä](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) tunnistettuja tiedostoja koskevat ilmoitukset.

> [!NOTE]
> ATP tarkistaa kaikki yksittäiset tiedostot SharePoint Onlinessa, OneDrivessa tai Microsoft Teamsissa. Tiedostot skannataan asynkronisesti käyttämällä jakamis-ja vieras toiminto tapahtumia sekä älykkään heuristiikkaa ja uhka signaaleja haitallisten tiedostojen tunnistamiseksi. Katso [SharePointin, OneDriven ja Microsoft teamsin ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).