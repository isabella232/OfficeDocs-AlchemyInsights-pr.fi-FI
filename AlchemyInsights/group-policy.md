---
title: Ryhmäkäytäntö
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256715"
---
# <a name="group-policy"></a><span data-ttu-id="edeb0-102">Ryhmäkäytäntö</span><span class="sxs-lookup"><span data-stu-id="edeb0-102">Group policy</span></span>

<span data-ttu-id="edeb0-103">Käyttäjä- ja tietokoneobjektien asetuksia Azure Active Directory -toimialueen palveluissa (Azure AD DS) hallitaan usein ryhmäkäytäntöobjektien (GPOs) avulla.</span><span class="sxs-lookup"><span data-stu-id="edeb0-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="edeb0-104">Azure AD DS sisältää sisäänrakennettuja GPOs-objekteja AADDC-käyttäjille ja AADDC-tietokonesäilöille.</span><span class="sxs-lookup"><span data-stu-id="edeb0-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="edeb0-105">Voit mukauttaa näitä sisäänrakennettuja ryhmäkäytäntöobjekteja ja määrittää ryhmäkäytännön tarpeen mukaan ympäristössäsi.</span><span class="sxs-lookup"><span data-stu-id="edeb0-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="edeb0-106">Azure AD DC -järjestelmänvalvojien ryhmän jäsenillä on ryhmäkäytäntöjen hallinnan oikeudet Azure AD DS -toimialueella, ja he voivat myös luoda mukautettuja ryhmäkäytäntöjä ja organisaatioyksiköitä.</span><span class="sxs-lookup"><span data-stu-id="edeb0-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="edeb0-107">Lisätietoja ryhmäkäytännön toiminnasta on ryhmäkäytännön [yleiskatsauksessa.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))</span><span class="sxs-lookup"><span data-stu-id="edeb0-107">For more information on what group policy is and how it works, see [Group Policy overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="edeb0-108">Yhdistelmäympäristössä paikalliseen AD DS -ympäristöön määritettyjä ryhmäkäytäntöjä ei synkronoida Azure AD DS:n kanssa.</span><span class="sxs-lookup"><span data-stu-id="edeb0-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="edeb0-109">Voit määrittää käyttäjien tai tietokoneiden määritysasetukset Azure AD DS:ssä muokkaamalla yhtä oletusarvoista ryhmäkäytäntöobjektia tai luomalla mukautetun ryhmäkäytäntöobjektin.</span><span class="sxs-lookup"><span data-stu-id="edeb0-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="edeb0-110">Tässä artikkelissa [ryhmäkäytännön hallinta](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) näyttää, miten voit asentaa ryhmäkäytäntöjen hallintatyökalut, miten voit muokata sisäänrakennettuja ryhmäkäytäntöobjekteja ja luoda mukautettuja ryhmäkäytäntöobjekteja.</span><span class="sxs-lookup"><span data-stu-id="edeb0-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>



