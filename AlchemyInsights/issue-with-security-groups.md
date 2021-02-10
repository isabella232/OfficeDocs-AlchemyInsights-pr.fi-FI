---
title: Ongelma käyttöoikeusryhmissä
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177493"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="8c581-102">Ongelma käyttöoikeusryhmissä</span><span class="sxs-lookup"><span data-stu-id="8c581-102">Issue with security groups</span></span>

<span data-ttu-id="8c581-103">**Jos saat verkkovirheen AADDS104**</span><span class="sxs-lookup"><span data-stu-id="8c581-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="8c581-104">Virheelliset verkon käyttöoikeusryhmän säännöt ovat yleisin azure Active Directory -toimialueen palveluiden (AD DS) verkkovirheiden syy.</span><span class="sxs-lookup"><span data-stu-id="8c581-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="8c581-105">Virtuaalisen verkon käyttöoikeusryhmän on sallittava tiettyjen porttien ja protokollien käyttö.</span><span class="sxs-lookup"><span data-stu-id="8c581-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="8c581-106">Jos nämä portit on estetty, Azure-ympäristö ei voi valvoa tai päivittää hallittua toimialuetta.</span><span class="sxs-lookup"><span data-stu-id="8c581-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="8c581-107">Tämä vaikuttaa myös Azure AD:n ja Azure AD DS:n väliseen synkronointiin.</span><span class="sxs-lookup"><span data-stu-id="8c581-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="8c581-108">Varmista, että oletusportit ovat avoinna, jotta palvelu ei keskeydy.</span><span class="sxs-lookup"><span data-stu-id="8c581-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="8c581-109">Lisätietoja yleisistä verkon käyttöoikeusryhmän määritysongelmista ja niiden ratkaisemisesta on kohdassa Käyttöoikeusryhmien lisääminen [ja tarkistaminen.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)</span><span class="sxs-lookup"><span data-stu-id="8c581-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
