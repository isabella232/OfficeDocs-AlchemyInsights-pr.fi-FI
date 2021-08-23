---
title: SMTP AUTH -asiakaslähetyksen TLS1.0- ja TLS 1.1 -protokollan poistaminen käytöstä
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13649"
- "9005383"
ms.openlocfilehash: 6751f4e8a177958fdec674899606252a4ae40a72
ms.sourcegitcommit: d9e6f700cd73a61c109e2a99bc71e559dba34722
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/18/2021
ms.locfileid: "58454769"
---
# <a name="disabling-tls10-and-tls-11-for-smtp-auth-client-submission"></a>SMTP AUTH -asiakaslähetyksen TLS1.0- ja TLS 1.1 -protokollan poistaminen käytöstä

Olemme äskettäin alkaneet poistaa TLS1.0- ja TLS 1.1 -käytöstä SMTP-AUTH-asiakaslähetyksessä. 

Jos olet määrittänyt laitteen, sovelluksen tai palvelimen, joka lähettää sähköpostia Microsoft 365 SMTP AUTH -sovelluslähetyksen menetelmällä, varmista, että laite, sovellus tai palvelin tukee SMTP:n TLS 1.2:ta. 