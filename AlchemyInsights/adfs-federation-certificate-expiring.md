---
title: ADFS Federation varmenteen vanhenemisen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: c608489be8497233d9d4f87ec53649026b823250
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28286751"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS Federation varmenteen vanhenemisen

Voit ratkaista tämän ongelman seuraavasti:
  
1. Asenna Microsoftin Azure Active Directory moduuli varten Windows PowerShell tietokoneeseen (Jos moduulia ei ole asennettu). Voit tehdä tämän Siirry [Hallitse Azure AD Windows PowerShellin avulla](https://aka.ms/aadposh).
    
2. Ohjeiden mukaisesti ”skenaario 1: AD FS-tunnussanoman allekirjoituksen sertifikaatti on vanhentunut” [Virhe ”virhe sivuston” liitetty käyttäjä kirjautuu sisään Office 365 ja Azure, Intune kun AD FS](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)-osassa.
    
3. [Kuinka päivittää tai korjata liitetty toimialue Office 365 ja Azure, Intune asetukset](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)noudattamalla.
    
    Lisätietoja Federation varmenteiden uusiminen, katso [Uusi Office 365 ja Azure Active Directory federation sertifikaatteja](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
    

