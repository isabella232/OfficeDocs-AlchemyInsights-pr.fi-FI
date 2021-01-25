---
title: Käyttäjän valmistelumääritteen yhdistäminen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949761"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="6d887-102">Käyttäjän valmistelumääritteen yhdistäminen</span><span class="sxs-lookup"><span data-stu-id="6d887-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="6d887-103">Lisätietoja tunnettujen määritteiden yhdistämisongelmien vianmäärityksestä on kohdassa [Määritteiden yhdistämismääritykset.](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings)</span><span class="sxs-lookup"><span data-stu-id="6d887-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="6d887-104">Microsoft Azure Active Directory (AD) tukee käyttäjien valmistelua kolmannen osapuolen SaaS-sovelluksille, kuten Salesforcelle, G Suitelle ja muille.</span><span class="sxs-lookup"><span data-stu-id="6d887-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="6d887-105">Jos otat käyttöön käyttäjän valmistelun kolmannen osapuolen SaaS-sovelluksessa, Azure-portaali ohjaa sen määritearvoja määritteiden yhdistämismääritysten avulla.</span><span class="sxs-lookup"><span data-stu-id="6d887-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="6d887-106">Lisätietoja oletusmääritteiden yhdistämismääritysten mukauttamisesta on kohdassa Käyttäjän valmistelumääritteiden yhdistämismääritysten [mukauttaminen SaaS-sovelluksissa Azure Active Directoryssa.](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes)</span><span class="sxs-lookup"><span data-stu-id="6d887-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="6d887-107">Lisätietoja SaaS-sovelluksen käyttäjien valmistelusta on ohjeaiheessa Mikä on automaattinen [SaaS-sovelluksen käyttäjien valmistelu Azure AD:ssä?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="6d887-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="6d887-108">Kun mukautat määritteiden yhdistämismäärityksiä käyttäjän valmistelua varten, saatat nähdä, että määrite, jonka haluat yhdistää, ei näy Lähdemäärite-luettelossa.</span><span class="sxs-lookup"><span data-stu-id="6d887-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="6d887-109">Synkronoi [määritteet](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) paikallisesta Active Directorysta Azure AD:n kanssa sovelluksen artikkeliin valmistelua varten. Näin voit lisätä puuttuvan määritteen synkronoimalla sen paikallisesta AD:stä Azure AD:lle.</span><span class="sxs-lookup"><span data-stu-id="6d887-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
