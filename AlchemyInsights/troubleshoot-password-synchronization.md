---
title: Salasanan synkronointiin liittyviä ongelmia
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
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732507"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="d93a1-102">Salasanan synkronointiin liittyviä ongelmia</span><span class="sxs-lookup"><span data-stu-id="d93a1-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="d93a1-103">Sellaisten ongelmien vianmääritys, joissa salasanoja ei synkronoida Azure AD Connectin version 1.1.614.0 tai uudemman kanssa:</span><span class="sxs-lookup"><span data-stu-id="d93a1-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="d93a1-104">Avaa uusi Windows PowerShell -istunto Azure AD Connect -palvelimessa **Suorita järjestelmänvalvojana** -asetuksen avulla.</span><span class="sxs-lookup"><span data-stu-id="d93a1-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="d93a1-105">Suorita **Set-ExecutionPolicy RemoteSigned** tai **Set-ExecutionPolicy rajoittamaton**.</span><span class="sxs-lookup"><span data-stu-id="d93a1-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="d93a1-106">Käynnistä ohjattu Azure AD Connect -toiminto.</span><span class="sxs-lookup"><span data-stu-id="d93a1-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="d93a1-107">Siirry **Lisätehtävät-sivulle,** valitse **Vianmääritys**ja valitse **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="d93a1-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="d93a1-108">Käynnistä Vianmääritys-valikon **vianmääritysvalikko PowerShellissä** valitsemalla Vianmääritys-sivulla Käynnistä.</span><span class="sxs-lookup"><span data-stu-id="d93a1-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="d93a1-109">Valitse päävalikosta **Salasanan synkronoinnin vianmääritys**.</span><span class="sxs-lookup"><span data-stu-id="d93a1-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="d93a1-110">Valitse alivalikosta **Salasanan synkronointi ei toimi lainkaan**.</span><span class="sxs-lookup"><span data-stu-id="d93a1-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="d93a1-111">**Tietoja vianmääritystehtävän tuloksista**</span><span class="sxs-lookup"><span data-stu-id="d93a1-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="d93a1-112">Vianmääritystehtävä suorittaa seuraavat tarkistukset:</span><span class="sxs-lookup"><span data-stu-id="d93a1-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="d93a1-113">Tarkistaa, että salasanan synkronointiominaisuus on käytössä Azure AD -vuokraajassa.</span><span class="sxs-lookup"><span data-stu-id="d93a1-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="d93a1-114">Tarkistaa, että Azure AD Connect -palvelin ei ole valmistelutilassa.</span><span class="sxs-lookup"><span data-stu-id="d93a1-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="d93a1-115">Kunkin paikallisen Active Directory -yhdistimen osalta (joka vastaa olemassa olevaa Active Directory -toimialuepuuryhmään):</span><span class="sxs-lookup"><span data-stu-id="d93a1-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="d93a1-116">Tarkistaa, että salasanan synkronointiominaisuus on käytössä.</span><span class="sxs-lookup"><span data-stu-id="d93a1-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="d93a1-117">Etsii salasanan synkronoinnin syketapahtumia Windowsin sovellustapahtumalokeista.</span><span class="sxs-lookup"><span data-stu-id="d93a1-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="d93a1-118">Kunkin paikallisen Active Directory -yhdistimen alla olevan Active Directory -toimialueen osalta:</span><span class="sxs-lookup"><span data-stu-id="d93a1-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="d93a1-119">Tarkistaa, että toimialue on tavoitettavissa Azure AD Connect -palvelimesta.</span><span class="sxs-lookup"><span data-stu-id="d93a1-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="d93a1-120">Tarkistaa, että paikallisen Active Directory -yhdistimen käyttämien Active Directory -toimialueen palveluiden (AD DS) tileillä on oikea käyttäjätunnus, salasana ja salasanasynkronointiin tarvittavat käyttöoikeudet.</span><span class="sxs-lookup"><span data-stu-id="d93a1-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="d93a1-121">Lisätietoja salasanan synkronoinnin vianmäärityksestä on [ohjeaiheessa Salasanan synkronoinnin vianmääritys Azure AD Connect -synkronoinnin kanssa](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="d93a1-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  