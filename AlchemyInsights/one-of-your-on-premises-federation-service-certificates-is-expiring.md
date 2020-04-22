---
title: Yksi paikallisista federation-palvelutodistuksistasi vanhenee
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 24c369c61ad7cf7a9fe101ac29271c32e5159c1f
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761380"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>Yksi paikallisista federation-palvelutodistuksistasi vanhenee

Voit ratkaista tämän ongelman seuraavasti:
  
- Asenna Windows PowerShellin Microsoft Azure Active Directory -moduuli tietokoneeseen (jos moduulia ei ole vielä asennettu). Voit tehdä tämän siirtymällä [Azure Active Directory PowerShell for Graphiin](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- Noudata AD FS:n skenaario1: AD FS -tunnuksen allekirjoitusvarmenne vanhentunut -osan ohjeita, [kun liitetty käyttäjä kirjautuu Office 365:een, Azureen tai Intuneen.](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)
    
- Noudata ohjeita kohdassa t[Liitetyn toimialueen asetusten päivittäminen tai korjaaminen Office 365:ssä, Azuressa tai Intunessa](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
Lisätietoja yhdistämisvarmenteiden uusimisesta on [ohjeaiheessa O365:n ja Azure AD:n varmenteiden uusiminen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

