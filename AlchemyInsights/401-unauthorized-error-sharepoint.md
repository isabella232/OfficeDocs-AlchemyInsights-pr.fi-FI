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
ms.openlocfilehash: ac2fe27a8e7b277bfaf18303bf5b792410a1ea6a
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539929"
---
# <a name="401-unauthorized-error-in-sharepoint"></a>401 Luvaton virhe SharePoint

Jos näyttöön tulee "(401) Unauthorized" -virhe SharePoint se voi olla liittyvä TLS 1.0/1.1 -käyttökoodin käytöstä poistoon. Lisätietoja: 

- [TLS 1.2:n valmistelu Office 365:ssä ja Office 365 GCC:ssä](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Todennusvirheitä ilmenee, jos asiakasohjelmalla ei ole TLS 1.2 -tukea](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Päivitys, jotta TLS 1.1 ja TLS 1.2 otetaan käyttöön WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Jos käyttäjät ovat Windows 7:ssä, varmista, että he tarkistavat [TLS Cipher Suites Windows 7:ssä.](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)