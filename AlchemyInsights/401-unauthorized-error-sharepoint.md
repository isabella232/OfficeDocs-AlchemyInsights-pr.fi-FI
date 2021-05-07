---
title: 401 Luvaton virhe SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: 6799b2112458a7ab3715c9b63e03c2c7ca3fe6be
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233495"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Luvaton virhe SharePoint

Jos näyttöön tulee "(401) Unauthorized" -virhe SharePoint se voi olla liittyvä TLS 1.0/1.1 -käyttökoodin käytöstä poistoon. Lisätietoja: 

[TLS 1.2:n valmistelu Office 365:ssä ja Office 365 GCC:ssä](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

[Todennusvirheitä ilmenee, jos asiakasohjelmalla ei ole TLS 1.2 -tukea](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

Jos käyttäjät ovat Windows 7:ssä, varmista, että he tarkistavat [TLS Cipher Suites Windows 7:ssä.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)