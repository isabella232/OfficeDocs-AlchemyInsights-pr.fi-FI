---
title: Toimialueen palvelun määrittäminen
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
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885224"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="d07d1-102">AAD-DS:n käyttöönotto ei onnistu tai käyttöönotto epäonnistuu</span><span class="sxs-lookup"><span data-stu-id="d07d1-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="d07d1-103">Voit ratkaista Azure AD -toimialueen palvelun (AAD-DS) käyttöönoton epäonnistumisen tai sen, että sitä ei ole otettu käyttöön, toimimalla seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="d07d1-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="d07d1-104">Jos käytät jo olemassa olevaa näennäisverkkoa, tarkista NSG:stä säännöt, jotka estävät portit, joita tarvitaan portaalin AAD-DS-synkronointiin. https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="d07d1-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="d07d1-105">Tarkista, onko virheilmoitukseen vastattu tässä vianmääritysoppaassa, joka on käytettävissä  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="d07d1-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="d07d1-106">Kokeile Azure AD -toimialueen palvelujen käyttöönottoa uudessa virtuaaliverkossa.</span><span class="sxs-lookup"><span data-stu-id="d07d1-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="d07d1-107">Tutustu AAD-DS:n käyttöönottoon aloitusoppaassa: [AAD-toimialuepalvelujen](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)luominen ja määrittäminen.</span><span class="sxs-lookup"><span data-stu-id="d07d1-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="d07d1-108">Jos sinulla on ongelmia Azure AD -toimialuepalvelujen käyttöönotossa, katso [Azure AD -toimialueen](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) palveluiden vianmääritys ja ratkaise yleisiä virheitä, jotta saat asiat toimimaan uudelleen.</span><span class="sxs-lookup"><span data-stu-id="d07d1-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="d07d1-109">**AAD-DS:n poistaminen käytöstä ei onnistu**</span><span class="sxs-lookup"><span data-stu-id="d07d1-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="d07d1-110">AAD-DS:tä ei voi keskeyttää.</span><span class="sxs-lookup"><span data-stu-id="d07d1-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="d07d1-111">Jos haluat lopettaa hallitun toimialueen käytön, se on poistettava.</span><span class="sxs-lookup"><span data-stu-id="d07d1-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="d07d1-112">Jos haluat poistaa hallitun toimialueen, katso [kohta AAD-toimialueen palvelun poistaminen.](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds)</span><span class="sxs-lookup"><span data-stu-id="d07d1-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



