---
title: Azure Active Directory -liitos
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9890"
ms.openlocfilehash: 59e3798131956847a61af2416c2e4210199cffa5
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404593"
---
# <a name="azure-active-directory-join"></a><span data-ttu-id="3f5d0-102">Azure Active Directory -liitos</span><span class="sxs-lookup"><span data-stu-id="3f5d0-102">Azure Active Directory join</span></span>

1. <span data-ttu-id="3f5d0-103">Jos määrität laiterekisteröintiä ensimmäistä kertaa, varmista, että olet tutustunut [Azure Active Directoryn](/azure/active-directory/devices/overview) laitehallinnan esittelyyn, joka opastaa sinua, miten saat hallitut laitteet Azure AD:lle.</span><span class="sxs-lookup"><span data-stu-id="3f5d0-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="3f5d0-104">Jos rekisteröit laitteita suoraan Azure AD:lle ja rekisteröit ne Intuneen, sinun on varmistettava, että olet määrittänyt [Intunen](/mem/intune/enrollment/device-enrollment) ja että käyttöoikeudet ovat käytössä ensin. [](/mem/intune/fundamentals/licenses-assign)</span><span class="sxs-lookup"><span data-stu-id="3f5d0-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](/mem/intune/enrollment/device-enrollment) and have the [licensing](/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="3f5d0-105">Varmista, että sinulla on oikeus suorittaa toimintoja Azure AD:ssä.</span><span class="sxs-lookup"><span data-stu-id="3f5d0-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="3f5d0-106">Vain Azure AD:n yleinen järjestelmänvalvoja voi hallita laiterekisteröinnin asetuksia.</span><span class="sxs-lookup"><span data-stu-id="3f5d0-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="3f5d0-107">Azure AD :n liittymisen käyttöönotto on ohjeaiheessa [Azure AD -liitoksen suunnittelu.](/azure/active-directory/devices/azureadjoin-plan)</span><span class="sxs-lookup"><span data-stu-id="3f5d0-107">To do Azure AD join implementation, see [Plan Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="3f5d0-108">Lisätietoja Azure AD -liitoksen yleisimpiä ongelmia ratkaisemisesta on Azure [Ad Joinin](/azure/active-directory/devices/faq) usein kysytyissä kysymyksissä ja Windows 10 Pro -laitteessa. Katso lisätietoja kohdasta Windows 10 Pro -koneeseen liittyminen Azure AD:lle ei onnistu – Päivitys on tarpeen [– Microsoft Community -yhteisöön.](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)</span><span class="sxs-lookup"><span data-stu-id="3f5d0-108">For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](/azure/active-directory/devices/faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).</span></span>
