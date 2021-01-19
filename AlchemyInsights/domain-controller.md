---
title: Toimialueen ohjauskone
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901022"
---
# <a name="domain-controller"></a><span data-ttu-id="0bbc4-102">Toimialueen ohjauskone</span><span class="sxs-lookup"><span data-stu-id="0bbc4-102">Domain controller</span></span>

<span data-ttu-id="0bbc4-103">**AAD-DS:n käyttöönotto ei onnistu tai käyttöönotto epäonnistuu**</span><span class="sxs-lookup"><span data-stu-id="0bbc4-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="0bbc4-104">Voit ratkaista Azure AD -toimialueen palvelun (AAD-DS) käyttöönoton epäonnistumisen tai sen, että sitä ei ole otettu käyttöön, toimimalla seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="0bbc4-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="0bbc4-105">Jos käytät jo olemassa olevaa näennäisverkkoa, tarkista NSG:stä säännöt, jotka estävät portit, joita tarvitaan portaalin AAD-DS-synkronointiin. https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="0bbc4-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="0bbc4-106">Tarkista, onko virheilmoitukseen vastattu tässä vianmääritysoppaassa, joka on käytettävissä  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="0bbc4-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="0bbc4-107">Kokeile Azure AD -toimialueen palvelujen käyttöönottoa uudessa virtuaaliverkossa.</span><span class="sxs-lookup"><span data-stu-id="0bbc4-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="0bbc4-108">Katso aloitusoppaasta, miten voit ottaa käyttöön AAD-DS:n, joka on saatavilla Azure AD -toimialuepalvelujen luontia [varten opetusohjelmassa.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)</span><span class="sxs-lookup"><span data-stu-id="0bbc4-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="0bbc4-109">Jos sinulla on ongelmia Azure AD -toimialuepalvelujen käyttöönotossa, katso [Azure AD -toimialueen](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) palveluiden vianmääritys ja ratkaise yleisiä virheitä, jotta saat asiat toimimaan uudelleen.</span><span class="sxs-lookup"><span data-stu-id="0bbc4-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="0bbc4-110">**AAD-DS:n poistaminen käytöstä ei onnistu**</span><span class="sxs-lookup"><span data-stu-id="0bbc4-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="0bbc4-111">AAD-DS:tä ei voi keskeyttää.</span><span class="sxs-lookup"><span data-stu-id="0bbc4-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="0bbc4-112">Jos haluat lopettaa hallitun toimialueen käytön, se on poistettava.</span><span class="sxs-lookup"><span data-stu-id="0bbc4-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="0bbc4-113">Jos ongelmia ilmenee, voit ratkaista yleisiä virhesanomia ja ohjeita vianmääritykseen, joiden avulla saat asiat taas toimimaan, artikkelista Azure Active Directory -toimialueen palveluiden [vianmääritys.](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="0bbc4-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>
