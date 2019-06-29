---
title: ADFS Federation varmenteen vanhenemisen
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
ms.openlocfilehash: b014e350d5f6f1a61feb223e3d3fd0a1f56f5872
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35357962"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS Federation varmenteen vanhenemisen

Voit ratkaista tämän ongelman seuraavasti:
  
1. Asenna Microsoftin Azure Active Directory moduuli varten Windows PowerShell tietokoneeseen (Jos moduulia ei ole asennettu). Voit tehdä tämän Siirry [Hallitse Azure AD Windows PowerShellin avulla](https://aka.ms/aadposh).

2. Ohjeiden mukaisesti ”skenaario 1: AD FS-tunnussanoman allekirjoituksen sertifikaatti on vanhentunut” [Virhe ”virhe sivuston” liitetty käyttäjä kirjautuu sisään Office 365 ja Azure, Intune kun AD FS](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)-osassa.

3. [Kuinka päivittää tai korjata liitetty toimialue Office 365 ja Azure, Intune asetukset](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)noudattamalla.

    Lisätietoja Federation varmenteiden uusiminen, katso [Uusi Office 365 ja Azure Active Directory federation sertifikaatteja](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
