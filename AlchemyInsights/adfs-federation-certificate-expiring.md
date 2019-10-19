---
title: ADFS Federation-sertifikaatti vanhenemassa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36737186"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS Federation-sertifikaatti vanhenemassa

Voit ratkaista tämän ongelman tekemällä seuraavat toimet:
  
1. Asenna Microsoft Azure Active Directory Module for Windows PowerShell tieto koneeseen (jos moduulia ei ole jo asennettu). Voit tehdä tämän siirtymällä [Azure AD:n hallintaan Windows PowerShellin avulla](https://aka.ms/aadposh).

2. Noudata "skenaario 1: AD FS Token-allekirjoitus varmenne vanhentunut"-osion ohjeita " [sivuston käyttämisessä"-virhe AD FS:ssä, kun Federated User kirjautuu Office 365-, Azure-tai Intune-käyttäjäksi](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. Noudata [Office 365-, Azure-tai Intune-tieto koneessa olevan Federated Domain-asetusten päivittäminen tai korjaaminen](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)-ohjeita.

    Lisä tietoja yhdistämisen varmenteiden uusimisesta [on artikkelissa Office 365: in ja Azure Active Directoryn yhdistämisen varmenteiden uusiminen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
