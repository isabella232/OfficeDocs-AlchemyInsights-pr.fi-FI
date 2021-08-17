---
title: Ota Lokero käyttöön SharePoint Onlinessa, OneDrive ja Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 7357f53ef7827aea9cbb0d222c338a5edf429ffd201bfbb6d7307b3d446fdae2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57894460"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Ota Lokero käyttöön SharePoint Onlinessa, OneDrive ja Microsoft Teams

1. Avaa yleisen järjestelmänvalvojan tai suojauksen järjestelmänvalvojan tunnistetietojen avulla Microsoft 365 Defender -portaali ja siirry sitten Käytännöt <https://security.microsoft.com> **&-sääntöjen** \>  \> **uhkien Lokero Käytännöt-osioon** 

   Siirry suoraan **Liitteet Lokero sivulle** käyttämällä <https://security.microsoft.com/safeattachmentv2> -painiketta.

2. Valitse **Lokero-sivulla** **Yleiset asetukset**.
3. Valitse näkyviin tulevassa pikaikkunassa **Ota Käyttöön Microsoft Defender for Office 365 for SharePoint OneDrive** ja Microsoft Teams ja valitse sitten **Tallenna**.

    > [!TIP]
    >
    > Voit parantaa Lokero liitteiden suojausta SharePoint OneDrive ja Microsoft Teams:
    >
    > - Voit estää käyttäjiä lataamasta haitallisia tiedostoja käyttämällä SharePoint `$true` Online PowerShellin **[Set-SPOTenant-cmdlet-komennon](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** *DisallowInfectedFileDownload-parametrin* arvoa. Lisätietoja on kohdassa [SharePoint lataamisen estäminen Online PowerShellin avulla.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)
    > - [Ilmoituskäytännön luominen havaittuja tiedostoja varten](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Lisätietoja on kohdassa Lokero [for Office 365 for SharePoint, OneDrive ja Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
