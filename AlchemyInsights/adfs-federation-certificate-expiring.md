---
title: ADFS-liittoutumisvarmenne vanhenee
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686711"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS-liittoutumisvarmenne vanhenee

Voit ratkaista ongelman seuraavasti:
  
1. Asenna Windows PowerShellin Microsoft Azure Active Directory -moduuli tietokoneeseen (jos moduulia ei ole vielä asennettu). Voit tehdä tämän menemään Azure [AD:n hallintaan Windows PowerShellin avulla.](https://aka.ms/aadposh)

2. Noudata "Skenaario 1: AD FS -tunnuksen allekirjoitusvarmenne vanhentunut" -osion "Sivuston käyttöongelma" -virheen ohjeita AD FS:ssä, kun liitetty käyttäjä kirjautuu [Microsoft 365:een, Azureen tai Intuneen.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)

3. Noudata ohjeita, jotka ovat kohdassa Liitetyn toimialueen asetusten päivittäminen tai [korjaaminen Microsoftissa, Azuressa tai Intunessa.](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)

    Lisätietoja liittousvarmentteiden uusimisesta on ohjeissa [Microsoft 365:n ja Azure Active Directoryn liittousvarmenteiden uusiminen.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)
