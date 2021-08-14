---
title: ADFS-liittoutumisvarmenteen vanheneminen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952966"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS-liittoutumisvarmenteen vanheneminen

Voit ratkaista ongelman seuraavasti:
  
1. Asenna Microsoft Azure Active Directory -Windows PowerShell tietokoneeseen (jos moduulia ei ole vielä asennettu). Voit tehdä tämän täällä: [Azure AD:n hallinta Windows PowerShell.](https://aka.ms/aadposh)

2. Noudata kohdan "Skenaario 1: AD FS -tunnuksen allekirjoitusvarmenne on vanhentunut" osassa "Sivuston käyttö on ongelma" -virhe AD FS:ssä, kun liitetty käyttäjä kirjautuu [Microsoft 365:een, Azureen tai Intuneen.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Noudata ohjeita kohdassa Liitetyn toimialueen asetusten päivittäminen tai korjaaminen [Microsoftissa, Azuressa tai Intunessa.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Lisätietoja liittousvarmentteiden uusimisesta on kohdassa Liittouksesi varmenteiden [uusiminen Microsoft 365 Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
