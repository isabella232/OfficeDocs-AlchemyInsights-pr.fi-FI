---
title: ADFS-liiton varmenteen vanheneminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710404"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS-liiton varmenteen vanheneminen

Voit ratkaista tämän ongelman seuraavasti:
  
1. Asenna Windows PowerShellin Microsoft Azure Active Directory -moduuli tietokoneeseen (jos moduulia ei ole vielä asennettu). Voit tehdä tämän siirtymällä kohtaan [Azure AD:n hallinta Windows PowerShellin avulla](https://aka.ms/aadposh).

2. Noudata AD FS:n skenaario1: AD FS -tunnuksen allekirjoitusvarmenne vanhentunut -osan ohjeita, [kun liitetty käyttäjä kirjautuu Microsoft 365:een, Azureen tai Intuneen.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Noudata ohjeaiheessa [Liitetyn toimialueen asetusten päivittäminen tai korjaaminen Microsoftissa, Azuressa tai Intunessa annettuja](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)ohjeita.

    Lisätietoja yhdistämisvarmenteiden uusimisesta on ohjeaiheessa [Microsoft 365:n ja Azure Active Directoryn yhdistämisvarmenteiden uusiminen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
