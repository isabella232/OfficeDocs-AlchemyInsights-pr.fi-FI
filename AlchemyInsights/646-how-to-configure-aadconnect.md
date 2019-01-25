---
title: 646 AADConnect määrittämisestä
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: e4ba295cd0661c3454180dd6a15895123840389e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499667"
---
# <a name="configure-sync-features"></a><span data-ttu-id="74004-102">Synkronoinnin ominaisuuksien määrittäminen</span><span class="sxs-lookup"><span data-stu-id="74004-102">Configure sync features</span></span>

<span data-ttu-id="74004-p101">Azure AD Connect on useita ominaisuuksia, jotka ovat oletusarvoisesti käytössä tai jotka voidaan ottaa käyttöön myöhemmin. Jotkin ominaisuudet edellyttävät lisämäärityksiä ympäristöissä.</span><span class="sxs-lookup"><span data-stu-id="74004-p101">Azure AD Connect includes several features that are enabled by default, or that you can enable later. Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="74004-p102">Azure AD [suodatus](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) rajoitusten objektit synkronoidaan. Tietokonetilit synkronoidaan oletusarvon, kaikki käyttäjät, yhteyshenkilöt, ryhmät ja Windows 10 mukaan. Voit sisällyttää tai jättää pois toimialueisiin, organisaatioyksiköihin tai muita määritteitä perustuvat objektit.</span><span class="sxs-lookup"><span data-stu-id="74004-p102">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD. By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized. You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="74004-p103">[Salasana hash synkronointi:](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) Synkronoi Azure AD paikalliseen Active Directory-salasanan hajautuksen. Tämä mahdollistaa salasanojen hallinta yhdessä paikassa, mutta käyttää samaa salasanaa molemmissa tiloissa ja solmuryhmän ympäristöissä. Active Directory on virallinen lähde, koska voit käyttää omia salasanakäytännöt.</span><span class="sxs-lookup"><span data-stu-id="74004-p103">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD. This allows password management in one location, but use of the same password in both on-premises and cloud environments. Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="74004-111">[Omatoiminen salasanan (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) käyttäjät voivat palauttaa omat salasanansa solmuryhmässä otettaessa yhteyttä paikalliseen Salasanakäytäntö edelleen.</span><span class="sxs-lookup"><span data-stu-id="74004-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="74004-112">[Takaisinkirjoitus laitteen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) avulla rekisteröity laitteet voidaan kirjoittaa takaisin paikalliseen Active Directoryyn, joten niitä voidaan käyttää ehdollisen käyttöoikeuden Azure AD.</span><span class="sxs-lookup"><span data-stu-id="74004-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="74004-p104">[Estä vahingossa poistaa](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) on oletusarvoisesti estämään liian monta samanaikaista objektin poistot (yli 500 objektien synkronointi kohti). Voit muuttaa tätä asetusta vastaamaan organisaation tarpeita.</span><span class="sxs-lookup"><span data-stu-id="74004-p104">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization). You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="74004-115">[Automaattinen päivitys](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) on käytössä oletusarvoisesti express asennukset ja varmistamaan Azure AD Yhdistä versio on aina ajan tasalla.</span><span class="sxs-lookup"><span data-stu-id="74004-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    

