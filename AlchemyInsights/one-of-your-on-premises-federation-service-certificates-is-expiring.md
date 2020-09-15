---
title: Yksi paikallisista liittoutumis palvelun varmenteista vanhenee
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
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: a4c78f3fdbba7786785f31098c9e80e77a165623
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673494"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="2c7cb-102">Yksi paikallisista liittoutumis palvelun varmenteista vanhenee</span><span class="sxs-lookup"><span data-stu-id="2c7cb-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="2c7cb-103">Voit korjata ongelman toimimalla seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="2c7cb-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="2c7cb-104">Asenna Windows PowerShellin Microsoft Azure Active Directory-moduuli tieto koneeseen (jos moduulia ei ole vielä asennettu).</span><span class="sxs-lookup"><span data-stu-id="2c7cb-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="2c7cb-105">Voit tehdä tämän siirtymällä [Azure Active Directory PowerShell for Graphiin ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="2c7cb-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="2c7cb-106">Seuraa "skenaario 1: AD FS-tunnuksen allekirjoitus varmenne vanhentunut"-osan ohjeita, joiden mukaan [sivuston käytössä ilmeni virhe AD FS:ssä, kun organisaation ulkopuolinen käyttäjä kirjautuu Microsoft 365-, Azure-tai Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)-järjestelmään.</span><span class="sxs-lookup"><span data-stu-id="2c7cb-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="2c7cb-107">Noudata ohjeita, jotka [liittyvät organisaation ulkopuolisen toimi alueen asetusten päivittämiseen tai korjaamiseen Microsoft 365-, Azure-tai Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)-sovelluksessa.</span><span class="sxs-lookup"><span data-stu-id="2c7cb-107">Follow the steps in [How to update or repair the settings of a federated domain in Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="2c7cb-108">Lisä tietoja liittämis varmenteiden uusimisesta on kohdassa [Varmenteen uusiminen O365 ja Azure](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)AD:ssä.</span><span class="sxs-lookup"><span data-stu-id="2c7cb-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

