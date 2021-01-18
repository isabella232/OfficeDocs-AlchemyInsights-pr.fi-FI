---
title: Toimialueen palvelusynkronointi
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885158"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="2f38a-102">Toimialueen palvelusynkronointi</span><span class="sxs-lookup"><span data-stu-id="2f38a-102">Domain service synchronization</span></span>

<span data-ttu-id="2f38a-103">Azure Active Directory -toimialueen palveluiden (Azure AD DS) hallitun toimialueen objektit ja tunnistetiedot voidaan luoda paikallisesti toimialueeseen tai synkronoida Azure Active Directory (Azure AD) -vuokraajan kautta.</span><span class="sxs-lookup"><span data-stu-id="2f38a-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="2f38a-104">Kun otat Azure AD DS:n käyttöön ensimmäistä kertaa, automaattinen yksipäinen synkronointi määritetään ja käynnistetään, jotta objektit replikoituvat Azure AD:stä.</span><span class="sxs-lookup"><span data-stu-id="2f38a-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="2f38a-105">Tämä yksitapainen synkronointi suoritetaan edelleen taustalla, jotta Azure AD DS:n hallittu toimialue pysyy ajan tasalla Azure AD:n muutosten kanssa.</span><span class="sxs-lookup"><span data-stu-id="2f38a-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="2f38a-106">Azure AD DS:stä ei tehdä synkronointia azure AD:n kanssa.</span><span class="sxs-lookup"><span data-stu-id="2f38a-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="2f38a-107">Lisätietoja Azure Active Directory -toimialueen palvelun synkronoinnista on [toimialuepalvelun synkronoinnissa.](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization)</span><span class="sxs-lookup"><span data-stu-id="2f38a-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
