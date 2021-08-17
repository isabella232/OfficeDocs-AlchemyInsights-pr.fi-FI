---
title: Taustalla oleva yhteys suljettiin -virhe SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: f0f82eaaa00d71992af445bb89346fb85bad3ade5d120b25ad3a6ea4f9674893
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/11/2021
ms.locfileid: "57883316"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>"Pohjana oleva yhteys suljettiin" -virhe SharePoint

Jos saat virhesanoman "Pohjana oleva yhteys suljettiin", SharePoint se saattaa olla yhteydessä TLS 1.0/1.1 -virheen poistoon. Lisätietoja on näissä artikkeleissa:

- [TLS 1.2:n valmistelu Office 365:ssä ja Office 365 GCC:ssä](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Todennusvirheitä ilmenee, jos asiakasohjelmalla ei ole TLS 1.2 -tukea](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Päivitys, jotta TLS 1.1 ja TLS 1.2 otetaan käyttöön WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Jos käyttäjät ovat Windows 7:ssä, varmista, että he tarkistavat [TLS Cipher Suites Windows 7:ssä.](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)