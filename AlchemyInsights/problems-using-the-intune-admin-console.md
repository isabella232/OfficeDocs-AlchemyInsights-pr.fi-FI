---
title: Ongelmia Intune-hallintakonsolin käytössä
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555038"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="2d237-102">Ongelmia Intune-hallintakonsolin käytössä</span><span class="sxs-lookup"><span data-stu-id="2d237-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="2d237-103">**"Käyttö estetty" siirryttäessä Intune-hallintaportaaliin.**</span><span class="sxs-lookup"><span data-stu-id="2d237-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="2d237-104">Jos olet Intune-mukautetun roolin jäsen, varmista, että tilillesi on määritetty Intune- tai Enterprise Mobility Suite (EMS) -käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="2d237-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="2d237-105">Jos käytät Configuration Manageria laitteiden hallintaan, varmista, ettet ole osa Configuration Managerin MDM:n Intune-käyttäjäkokoelmaa.</span><span class="sxs-lookup"><span data-stu-id="2d237-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="2d237-106">Varmista, että sinulle on määritetty asianmukaiset roolipohjaiset hallintaoikeudet (RBAC) Intune roles -terässä.</span><span class="sxs-lookup"><span data-stu-id="2d237-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="2d237-107">Varmista, että käytetty ryhmä ei ole jakeluluettelo.</span><span class="sxs-lookup"><span data-stu-id="2d237-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="2d237-108">Azure-portaalin Intune tukee vain Azure Active Directory -käyttöoikeusryhmiin kuuluvia käyttäjätilejä.</span><span class="sxs-lookup"><span data-stu-id="2d237-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="2d237-109">Tarkastele ryhmiä Azure-portaalissa > **Intune**  >  **Groupsissa**tai Azure-portaalissa > **Azure Active Directoryssa**.</span><span class="sxs-lookup"><span data-stu-id="2d237-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="2d237-110">**Käyttäjällä on liian monta intune-roolin käyttöoikeuksia**</span><span class="sxs-lookup"><span data-stu-id="2d237-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="2d237-111">Kehota käyttäjää siirtymään **Intune**  >  **Intune -rooleihin**  >  **Omat oikeudet**  >  **Vie** tarkistaaksesi myönnetyt käyttöoikeudet.</span><span class="sxs-lookup"><span data-stu-id="2d237-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="2d237-112">**Lisäsin rooliin vaikutusalueryhmän, mutta kyseisen roolin käyttäjät näkevät edelleen muita käyttäjiä tai laitteita.**</span><span class="sxs-lookup"><span data-stu-id="2d237-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="2d237-113">Vaikutusalueryhmät eivät suodata käyttäjiä tai laitteita.</span><span class="sxs-lookup"><span data-stu-id="2d237-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="2d237-114">Vaikutusalueryhmät:</span><span class="sxs-lookup"><span data-stu-id="2d237-114">Scope groups:</span></span>

- <span data-ttu-id="2d237-115">Rajoita, kenelle käyttäjät voivat määrittää käytäntöjä tai sovelluksia.</span><span class="sxs-lookup"><span data-stu-id="2d237-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="2d237-116">Salli vain tiettyjen käyttäjien suorittaa etätehtäviä laitteissa.</span><span class="sxs-lookup"><span data-stu-id="2d237-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="2d237-117">Lisätietoja vaikutusalueryhmistä on kohdassa [Roolipohjainen käytönvalvonta (RBAC) Ja Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="2d237-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="2d237-118">**Lisäsin käyttäjän Intune rooli, mutta heillä on edelleen täysi pääsy Intune admin konsoli.**</span><span class="sxs-lookup"><span data-stu-id="2d237-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="2d237-119">Siirry Azure-portaalin Intune > **-kohtaan** ja varmista, että käyttäjää ei ole määritetty mihinkään seuraavista azure-portaalin rooleista:</span><span class="sxs-lookup"><span data-stu-id="2d237-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="2d237-120">Yleinen järjestelmänvalvoja</span><span class="sxs-lookup"><span data-stu-id="2d237-120">Global administrator</span></span>
- <span data-ttu-id="2d237-121">Intune-palvelun järjestelmänvalvoja</span><span class="sxs-lookup"><span data-stu-id="2d237-121">Intune service administrator</span></span>
- <span data-ttu-id="2d237-122">SharePoint-järjestelmänvalvoja</span><span class="sxs-lookup"><span data-stu-id="2d237-122">SharePoint administrator</span></span>

<span data-ttu-id="2d237-123">Lisätietoja on [ohjeaiheessa Roolipohjainen käytönvalvonta (RBAC) Ja Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="2d237-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="2d237-124">**Käyttöongelmat**</span><span class="sxs-lookup"><span data-stu-id="2d237-124">**Access Issues**</span></span>

<span data-ttu-id="2d237-125">Lisätietoja on [ohjeaiheessa Office 365:ssä, Azuressa tai Intunessa kirjautuminen ei onnistu.](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)</span><span class="sxs-lookup"><span data-stu-id="2d237-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>