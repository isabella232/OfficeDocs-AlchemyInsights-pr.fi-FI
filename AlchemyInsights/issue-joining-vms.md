---
title: Ongelma liittyminen VMS:iin
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885212"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="9d7ad-102">Ongelma liittyminen VMS:iin</span><span class="sxs-lookup"><span data-stu-id="9d7ad-102">Issue joining VMs</span></span>

<span data-ttu-id="9d7ad-103">Voit ratkaista ongelmia, jotka ilmenevät, kun yrität liittyä VMS-isiin, toimimalla seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="9d7ad-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="9d7ad-104">Yritä kirjautua sisään **UPN-muodossa** (esimerkiksi "joeuser@contoso.com") **SAMAccountName-muodon** (CONTOSO\joeuser) sijaan.</span><span class="sxs-lookup"><span data-stu-id="9d7ad-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="9d7ad-105">Varmista, että olet ottanut salasanasynkronoinnin käyttöön aloitusoppaan *ohjeiden* mukaisesti.</span><span class="sxs-lookup"><span data-stu-id="9d7ad-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="9d7ad-106">Varmista, että kyseinen käyttäjätili ei ole ulkoinen tili Azure AD -vuokraajassa.</span><span class="sxs-lookup"><span data-stu-id="9d7ad-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="9d7ad-107">Ulkoiset käyttäjät eivät voi kirjautua hallittuun toimialueeseen, koska Azure AD -toimialuepalveluilla ei ole tällaisten käyttäjätilien tunnistetietoja.</span><span class="sxs-lookup"><span data-stu-id="9d7ad-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="9d7ad-108">Jos kyseinen käyttäjätili on vain pilvipalvelun käyttäjätili, varmista, että käyttäjät ovat vaihtaneet salasanansa Azure AD -toimialueen palveluiden käytön jälkeen.</span><span class="sxs-lookup"><span data-stu-id="9d7ad-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="9d7ad-109">Tämä vaihe aiheuttaa Azure AD -toimialuepalvelujen edellyttämät tunnistetietojen hasheet.</span><span class="sxs-lookup"><span data-stu-id="9d7ad-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="9d7ad-110">Jos ongelmaan liittyvät käyttäjätilit synkronoidaan paikallisesta hakemistosta, varmista, että Azure AD Connectin suositeltu julkaisu on määritetty suorittamaan täysi synkronointi.</span><span class="sxs-lookup"><span data-stu-id="9d7ad-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="9d7ad-111">Jos ongelmat jatkuvat vaiheen 4 vahvistuksen jälkeen, suorita seuraavat komennot synkronointikoneesta:</span><span class="sxs-lookup"><span data-stu-id="9d7ad-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="9d7ad-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="9d7ad-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>