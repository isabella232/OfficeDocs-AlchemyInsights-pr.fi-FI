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
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801044"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Microsoft Defenderin ottaminen käyttöön Office 365 for SharePoint Onlinessa, OneDrivessa ja Microsoft Teamsissa

1. Siirry kohtaan https://protection.office.com ja Kirjaudu sisään.
2. Valitse **uhkien hallinta**  >  **käytännön**  >  **turvalliset liitteet** .
3. Valitse **Ota SharePoint-, OneDrive-ja Microsoft TEAMSIN ATP käyttöön** ja valitse sitten **Tallenna** .
4. Suositellut Jos sinulla on yleinen järjestelmänvalvojana tai SharePoint Online-järjestelmänvalvojana, suorita [-spoalion cmdlet-](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) komentosovelma, jonka **Disallowinfectedfiledownload** -parametrin arvona on *True* .
5. Suositellut [Määritä](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) tunnistettuja tiedostoja koskevat ilmoitukset.

> [!NOTE]
> ATP tarkistaa kaikki yksittäiset tiedostot SharePoint Onlinessa, OneDrivessa tai Microsoft Teamsissa. Tiedostot skannataan asynkronisesti käyttämällä jakamis-ja vieras toiminto tapahtumia sekä älykkään heuristiikkaa ja uhka signaaleja haitallisten tiedostojen tunnistamiseksi. Katso [SharePointin, OneDriven ja Microsoft teamsin ATP](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).