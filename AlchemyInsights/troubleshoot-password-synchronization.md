---
title: Salasanojen synkronoinnin vianmääritys
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
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2019
ms.locfileid: "28287141"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="f4f9f-102">Salasanojen synkronoinnin vianmääritys</span><span class="sxs-lookup"><span data-stu-id="f4f9f-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="f4f9f-103">Jos ei ole salasanoja ovat synkronoituna Azure AD Yhdistä versio 1.1.614.0 tai uudempi ongelmien vianmääritys:</span><span class="sxs-lookup"><span data-stu-id="f4f9f-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="f4f9f-104">Avaa uuden Windows PowerShell-istunnon Azure AD yhteyden palvelimeen ja **Suorita järjestelmänvalvojana** -asetusta.</span><span class="sxs-lookup"><span data-stu-id="f4f9f-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="f4f9f-105">Suorita **Set-suorituskäytäntöä RemoteSigned** tai **Set-suorituskäytäntöä rajoittamaton**.</span><span class="sxs-lookup"><span data-stu-id="f4f9f-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="f4f9f-106">Käynnistä ohjattu Azure AD-muodosta.</span><span class="sxs-lookup"><span data-stu-id="f4f9f-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="f4f9f-107">Siirry \*\* lisätehtävät \*\*-sivulla \*\* vianmääritys \*\*, ja valitse **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="f4f9f-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="f4f9f-108">Vianmääritys sivulla **vianmäärityksen käynnistäminen Käynnistä** -valikosta PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f4f9f-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="f4f9f-109">Valitse päävalikosta, **Salasanojen synkronoinnin vianmäärityksestä**.</span><span class="sxs-lookup"><span data-stu-id="f4f9f-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="f4f9f-110">Sub-valikosta Valitse **salasana ei toimi ollenkaan**.</span><span class="sxs-lookup"><span data-stu-id="f4f9f-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="f4f9f-111">**Tietoja vianmäärityksen tehtävän tulokset**</span><span class="sxs-lookup"><span data-stu-id="f4f9f-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="f4f9f-112">Vianetsinnän tehtävän suorittaa seuraavat tarkistukset:</span><span class="sxs-lookup"><span data-stu-id="f4f9f-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="f4f9f-113">Tarkistaa, että salasana synkronointitoiminnon Azure AD-vuokralaisen on käytössä.</span><span class="sxs-lookup"><span data-stu-id="f4f9f-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="f4f9f-114">Vahvistaa Azure AD Yhdistä palvelimeen ei väliaikaisen tilassa.</span><span class="sxs-lookup"><span data-stu-id="f4f9f-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="f4f9f-115">Jokaisen aiemmin paikalliseen Active Directory Connector (joka vastaa Active Directory-toimialuepuuryhmän):</span><span class="sxs-lookup"><span data-stu-id="f4f9f-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="f4f9f-116">Tarkistaa, että salasana synkronointi-ominaisuus on käytössä.</span><span class="sxs-lookup"><span data-stu-id="f4f9f-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="f4f9f-117">Etsii salasana syke synkronointitapahtumat Windowsin sovellus-tapahtumalokiin.</span><span class="sxs-lookup"><span data-stu-id="f4f9f-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="f4f9f-118">Varten kukin Active Directory-toimialueen paikalliseen Active Directory connector-kohdassa:</span><span class="sxs-lookup"><span data-stu-id="f4f9f-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="f4f9f-119">Tarkistaa, että toimialue on käytettävissä Azure AD Yhdistä palvelimeen.</span><span class="sxs-lookup"><span data-stu-id="f4f9f-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="f4f9f-120">Vahvistaa, että paikallinen Active Directory connector käyttää Active Directory Domain Services (AD DS)-tilit on oikea käyttäjänimi, salasana ja salasanan synkronointia varten tarvittavat oikeudet.</span><span class="sxs-lookup"><span data-stu-id="f4f9f-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="f4f9f-121">Salasanan synkronointi vianmäärityksen lisäapua Katso [vianmääritys salasanojen synkronoinnin Azure AD Yhdistä synkronoinnissa](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="f4f9f-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

