---
title: Järjestelmänvalvojien lisääminen ja hallinta – MCA FL/CL
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7424"
ms.openlocfilehash: f5791cb12e565cb04f7ac6bc9bb401fcca3e4e9e
ms.sourcegitcommit: dd9eb38bf9403de29f46c844cb64bc1d4c515afc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692114"
---
# <a name="how-to-add-and-manage-admins---mca-flcl"></a><span data-ttu-id="444c3-102">Järjestelmänvalvojien lisääminen ja hallinta – MCA FL/CL</span><span class="sxs-lookup"><span data-stu-id="444c3-102">How to add and manage admins - MCA FL/CL</span></span>

<span data-ttu-id="444c3-103">Jos haluat hallita Microsoft-asiakas sopimusta (MCA), voit käyttää eri rooleja, joilla on haluttu käyttö oikeus taso.</span><span class="sxs-lookup"><span data-stu-id="444c3-103">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="444c3-104">Nämä roolit ovat niiden sisäisten Azure-palvelu roolien lisäksi, joiden avulla voit hallita resurssejasi.</span><span class="sxs-lookup"><span data-stu-id="444c3-104">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="444c3-105">**Voit lisätä laskutus rooleja Azure-portaalissa seuraavasti:**</span><span class="sxs-lookup"><span data-stu-id="444c3-105">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="444c3-106">Kirjaudu sisään Azure- [portaaliin](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="444c3-106">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="444c3-107">Hae *kustannusten hallinta + laskutus*.</span><span class="sxs-lookup"><span data-stu-id="444c3-107">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="444c3-108">Valitse käytön hallinta (IAM) sellaisen käyttö alueen mukaan, kuten laskutus tili, laskutus profiili tai laskun osa, jossa haluat myöntää käyttö oikeuden.</span><span class="sxs-lookup"><span data-stu-id="444c3-108">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="444c3-109">Käyttö oikeuksien hallinta-sivulla on lueteltu käyttäjät ja ryhmät, jotka on määritetty kullekin roolille kyseiselle alueelle.</span><span class="sxs-lookup"><span data-stu-id="444c3-109">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="444c3-110">Jos haluat antaa käyttäjälle käyttö oikeuden, valitse **Lisää** sivun yläreunasta.</span><span class="sxs-lookup"><span data-stu-id="444c3-110">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="444c3-111">Valitse rooli avattavasta *rooli* -luettelosta.</span><span class="sxs-lookup"><span data-stu-id="444c3-111">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="444c3-112">Kirjoita sen käyttäjän Sähkö posti osoite, jolle haluat myöntää käyttö oikeuden.</span><span class="sxs-lookup"><span data-stu-id="444c3-112">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="444c3-113">Määritä rooli valitsemalla **Tallenna** .</span><span class="sxs-lookup"><span data-stu-id="444c3-113">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="444c3-114">Jos haluat poistaa käyttäjän käyttö oikeuden, valitse käyttäjä, jonka rooli määritystä haluat poistaa.</span><span class="sxs-lookup"><span data-stu-id="444c3-114">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="444c3-115">Valitse **Poista**.</span><span class="sxs-lookup"><span data-stu-id="444c3-115">Select **Remove**.</span></span>

<span data-ttu-id="444c3-116">**Suositellut asia kirjat**</span><span class="sxs-lookup"><span data-stu-id="444c3-116">**Recommended Documents**</span></span>

- [<span data-ttu-id="444c3-117">Laskutus rooli määritykset</span><span class="sxs-lookup"><span data-stu-id="444c3-117">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="444c3-118">Laskutus tilin roolit ja tehtävät</span><span class="sxs-lookup"><span data-stu-id="444c3-118">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="444c3-119">MCA-laskutus tilin käytön aloittaminen</span><span class="sxs-lookup"><span data-stu-id="444c3-119">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="444c3-120">Microsoft-asiakas sopimuksen käytön tarkistaminen</span><span class="sxs-lookup"><span data-stu-id="444c3-120">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
