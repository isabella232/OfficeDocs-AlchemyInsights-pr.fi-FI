---
title: Azure Active Directoryn yhdistelmäliittämän vianmääritys
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401904"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="9a52b-102">Azure Active Directoryn yhdistelmäliittämän vianmääritys</span><span class="sxs-lookup"><span data-stu-id="9a52b-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="9a52b-103">Erittäin suositeltavaa: varmista, että laite voi käyttää järjestelmätilin laiterekisteröinnin päätepisteitä käyttämällä komentosarjaa [Testaa laiterekisteröinnin yhteyttä](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span><span class="sxs-lookup"><span data-stu-id="9a52b-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="9a52b-104">Jos määrität laiterekisteröintiä ensimmäistä kertaa, muista tarkistaa [Johdanto Azure Active Directoryn laitehallintaan](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/), jotta saat lisätietoja laitteiden hallinnasta Azure AD:ssä.</span><span class="sxs-lookup"><span data-stu-id="9a52b-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="9a52b-105">Jos rekisteröit laitteita suoraan Azure Active Directoryyn ja kirjaat ne Intuneen, varmista ensin, että olet [määrittänyt Intunen](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) ja että [käyttöoikeudet](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) ovat kunnossa.</span><span class="sxs-lookup"><span data-stu-id="9a52b-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="9a52b-106">Varmista, että sinulla on oikeus suorittaa toimintoja Azure AD:ssä ja paikallisessa AD:ssä.</span><span class="sxs-lookup"><span data-stu-id="9a52b-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="9a52b-107">Vain Azure AD:n yleinen järjestelmänvalvoja voi hallita laiterekisteröinnin asetuksia.</span><span class="sxs-lookup"><span data-stu-id="9a52b-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="9a52b-108">Lisäksi jos määrität automaattisia rekisteröintejä paikalliseen Active Directoryyn, sinun on oltava Active Directoryn ja AD FS:n järjestelmänvalvoja (jos sovellettavissa).</span><span class="sxs-lookup"><span data-stu-id="9a52b-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="9a52b-109">Lisätietoja yhdistelmäliittämän mahdollisten ongelmien ratkaisemisesta on kohdassa [Yhdistelmäliittämän vianmääritys](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current); lisätietoja Azure AD:n yhdistelmäliittämän määrittämisestä ja laitteiden hallinnasta Azure AD -portaalissa on kohdissa [Azure AD:n yhdistelmäliittämän laitteiden määrittäminen (paikalliseen toimialueeseen liitetyt)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) ja [Laitteiden hallinta Azure-portaalissa](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="9a52b-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="9a52b-110">Ratkaisuja yleisiin Azure Active Directoryn yhdistelmäliittämän ongelmiin on kohdassa [Azure AD:n yhdistelmäliittämän usein kysytyt kysymykset](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span><span class="sxs-lookup"><span data-stu-id="9a52b-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
