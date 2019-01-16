---
title: Yksi paikallinen Federation palvelun varmenteita on päättyvän
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 89a4dd910d43d70e849be19d5f88e281f6d19834
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28286491"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="65e0d-102">Yksi paikallinen Federation palvelun varmenteita on päättyvän</span><span class="sxs-lookup"><span data-stu-id="65e0d-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="65e0d-103">Voit ratkaista tämän ongelman seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="65e0d-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="65e0d-p101">Asenna Microsoftin Azure Active Directory moduuli varten Windows PowerShell tietokoneeseen (Jos moduulia ei ole asennettu). Voit tehdä tämän Siirry [Graph Azure Active Directory-PowerShell](https://docs.microsoft.com/en-us/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="65e0d-p101">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed). To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/en-us/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="65e0d-106">Ohjeiden mukaisesti ”skenaario 1: AD FS-tunnussanoman allekirjoituksen sertifikaatti on vanhentunut” [Virhe ”virhe sivuston” liitetty käyttäjä kirjautuu sisään Office 365 ja Azure, Intune kun AD FS](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)-osassa.</span><span class="sxs-lookup"><span data-stu-id="65e0d-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/en-us/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="65e0d-107">T[miten päivittää tai korjata liitetty toimialue Office 365 ja Azure, Intune asetukset](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)noudattamalla.</span><span class="sxs-lookup"><span data-stu-id="65e0d-107">Follow the steps in t[How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/en-us/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="65e0d-108">Saat lisätietoja Federation varmenteiden uusiminen [Sertifikaattien uusimisen Azure Mainos-ja O365](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span><span class="sxs-lookup"><span data-stu-id="65e0d-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

