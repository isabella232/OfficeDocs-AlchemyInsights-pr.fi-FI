---
title: Päätepiste DLP:tä ei ole otettu käyttöön käyttäjän laitteessa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731411"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a>Päätepiste DLP:tä ei ole otettu käyttöön käyttäjän laitteessa

Jos Endpoint-tietojen menetyksen estämisasetus (DLP) ei ole käytössä käyttäjän laitteessa, varmista, että täytät seuraavat vaatimukset:

- Windows 10 x64 koontiversio 1809 tai uudempi on asennettu laitteeseen.
- Haittaohjelmien torjuntaohjelman versio 4.18.2009.7 tai uudempi on asennettu.
- Laite on **jokin** seuraavista:
    
    - Azure Active Directory (Azure AD) liitetty
    - Azure AD -yhdistelmäympäristö liitetty
    - Rekisteröity AAD

- Jos haluat pakottaa käytäntötoiminnot, varmista, että Microsoft Chromium Edge -selain on asennettu päätepistelaitteeseen.

Lisätietoja Endpoint DLP:n käyttöönottovaatimuksista on kohdassa [Endpoint-tietojen menetyksen estämisen käytön aloittaminen.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)