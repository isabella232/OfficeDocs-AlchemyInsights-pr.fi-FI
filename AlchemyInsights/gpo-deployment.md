---
title: GPO-käyttöönotto
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427255"
---
# <a name="gpo-deployment"></a><span data-ttu-id="48f1a-102">GPO-käyttöönotto</span><span class="sxs-lookup"><span data-stu-id="48f1a-102">GPO Deployment</span></span>

<span data-ttu-id="48f1a-103">Käyttäjä- ja tietokoneobjektien asetuksia Azure Active Directory -toimialueen palveluissa (Azure AD DS) hallitaan usein ryhmäkäytäntöobjektien (GPOs) avulla.</span><span class="sxs-lookup"><span data-stu-id="48f1a-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="48f1a-104">Azure AD DS sisältää sisäänrakennettuja GPOs-objekteja AADDC-käyttäjille ja AADDC-tietokonesäilöille.</span><span class="sxs-lookup"><span data-stu-id="48f1a-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="48f1a-105">Voit mukauttaa näitä sisäänrakennettuja ryhmäkäytäntöobjekteja ja määrittää ryhmäkäytännön tarpeen mukaan ympäristössäsi.</span><span class="sxs-lookup"><span data-stu-id="48f1a-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="48f1a-106">Azure AD DC -järjestelmänvalvojien ryhmän jäsenillä on ryhmäkäytäntöjen hallinnan oikeudet Azure AD DS -toimialueella, ja he voivat myös luoda mukautettuja ryhmäkäytäntöjä ja organisaatioyksiköitä.</span><span class="sxs-lookup"><span data-stu-id="48f1a-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="48f1a-107">Lisätietoja ryhmäkäytännön toiminnasta on ryhmäkäytännön [yleiskatsauksessa.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))</span><span class="sxs-lookup"><span data-stu-id="48f1a-107">For more information on what group policy is and how it works, see [Group Policy Overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="48f1a-108">Yhdistelmäympäristössä paikalliseen AD DS -ympäristöön määritettyjä ryhmäkäytäntöjä ei synkronoida Azure AD DS:n kanssa.</span><span class="sxs-lookup"><span data-stu-id="48f1a-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="48f1a-109">Voit määrittää käyttäjien tai tietokoneiden määritysasetukset Azure AD DS:ssä muokkaamalla yhtä oletusarvoista ryhmäkäytäntöobjektia tai luomalla mukautetun ryhmäkäytäntöobjektin.</span><span class="sxs-lookup"><span data-stu-id="48f1a-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="48f1a-110">Tässä artikkelissa [ryhmäkäytännön hallinta](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) näyttää, miten voit asentaa ryhmäkäytäntöjen hallintatyökalut, miten voit muokata sisäänrakennettuja ryhmäkäytäntöobjekteja ja luoda mukautettuja ryhmäkäytäntöobjekteja.</span><span class="sxs-lookup"><span data-stu-id="48f1a-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>
