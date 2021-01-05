---
title: Järjestelmänvalvojien lisääminen ja hallinta – Suositellut vaiheet
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755832"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a><span data-ttu-id="71510-102">Järjestelmänvalvojien lisääminen ja hallinta – Suositellut vaiheet</span><span class="sxs-lookup"><span data-stu-id="71510-102">How to add and manage administrators - recommended steps</span></span>

<span data-ttu-id="71510-103">Ongelman kuva uksen perusteella olemme löytäneet ratkaisun.</span><span class="sxs-lookup"><span data-stu-id="71510-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="71510-104">Useimmat Asiakkaat pystyivät ratkaisemaan ongelmaansa sen jälkeen, kun he ovat seuraavat asia kirjojamme.</span><span class="sxs-lookup"><span data-stu-id="71510-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="71510-105">**Tila uksen valvojan tai Yhteishallinnoijan muokkaaminen**</span><span class="sxs-lookup"><span data-stu-id="71510-105">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="71510-106">Tilin järjestelmänvalvoja voi muokata molempia rooleja, mutta tila uksen järjestelmänvalvoja voi muuttaa vain yhteisjärjestelmänvalvojia Azure- [portaalissa](https://ms.portal.azure.com/#home).</span><span class="sxs-lookup"><span data-stu-id="71510-106">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="71510-107">Azure-tila uksen järjestelmänvalvojien lisääminen tai muuttaminen</span><span class="sxs-lookup"><span data-stu-id="71510-107">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="71510-108">**Tila uksen valvojan tai sisäisten (OLEVINAAN) tilausten Co-Administrator päivittäminen**</span><span class="sxs-lookup"><span data-stu-id="71510-108">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="71510-109">Palvelun hallinnoija tai Yhteishallinnoija voi itse palvella tätä toimintoa seuraavien vaiheiden avulla:</span><span class="sxs-lookup"><span data-stu-id="71510-109">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="71510-110">Kirjaudu sisään Azure- [portaaliin](https://ms.portal.azure.com/#home) ja valitse vasemman reunan **kustannusten hallinta + laskutus** .</span><span class="sxs-lookup"><span data-stu-id="71510-110">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="71510-111">Napsauta tilaustasi koskevaa rivi kohdetta.</span><span class="sxs-lookup"><span data-stu-id="71510-111">Click on the line item with your subscription.</span></span> <span data-ttu-id="71510-112">Tämä avaa tila uksen yleiskatsauksen.</span><span class="sxs-lookup"><span data-stu-id="71510-112">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="71510-113">Valitse **tila uksen** Blade-kohdassa **Ominaisuudet**.</span><span class="sxs-lookup"><span data-stu-id="71510-113">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="71510-114">Napsauta **palvelun järjestelmänvalvoja** -painiketta.</span><span class="sxs-lookup"><span data-stu-id="71510-114">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="71510-115">Kirjoita sen käyttäjän Sähkö posti viesti, jonka haluat määrittää palvelun järjestelmänvalvojaksi, ja valitse **OK**.</span><span class="sxs-lookup"><span data-stu-id="71510-115">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="71510-116">**Yhteishallinnoijan lisääminen/muuttaminen tai poistaminen**</span><span class="sxs-lookup"><span data-stu-id="71510-116">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="71510-117">Kirjaudu [Azure-portaaliin](https://ms.portal.azure.com/#home) palvelun järjestelmänvalvojana.</span><span class="sxs-lookup"><span data-stu-id="71510-117">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="71510-118">Avaa [tila ukset](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) ja valitse tilaus.</span><span class="sxs-lookup"><span data-stu-id="71510-118">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="71510-119">(Co-adminstrators voidaan määrittää vain tila uksen laajuus-kohdassa.)</span><span class="sxs-lookup"><span data-stu-id="71510-119">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="71510-120">Siirtyminen **käyttö oikeuksien hallintaan (IAM)**  >  **perinteiset järjestelmänvalvojat**  >  **Lisää**  >  **yhteisjärjestelmänvalvoja** -ruudun avaaminen Lisää  yhteisjärjestelmänvalvojan valinta ruutu (jos lisää yhteisjärjestelmänvalvoja-vaihto ehto ei ole käytössä, se tarkoittaa, että sinulla ei ole käyttö oikeuksia).</span><span class="sxs-lookup"><span data-stu-id="71510-120">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="71510-121">Valitse käyttäjä, jonka haluat lisätä, ja valitse **Lisää**.</span><span class="sxs-lookup"><span data-stu-id="71510-121">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="71510-122">**Opi lisää:**</span><span class="sxs-lookup"><span data-stu-id="71510-122">**Learn more:**</span></span>
- [<span data-ttu-id="71510-123">Yhteishallinnoijan lisääminen</span><span class="sxs-lookup"><span data-stu-id="71510-123">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="71510-124">Yhteishallinnoijan poistaminen</span><span class="sxs-lookup"><span data-stu-id="71510-124">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="71510-125">Palvelun valvojan vaihtaminen</span><span class="sxs-lookup"><span data-stu-id="71510-125">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="71510-126">Tilin valvojan tarkasteleminen</span><span class="sxs-lookup"><span data-stu-id="71510-126">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="71510-127">Käytön hallinta RBAC-ja Azure-portaalin avulla</span><span class="sxs-lookup"><span data-stu-id="71510-127">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="71510-128">**Käyttäjien lisääminen tai poistaminen Azure Active Directoryssa (AD)**</span><span class="sxs-lookup"><span data-stu-id="71510-128">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="71510-129">Voit lisätä uusia käyttäjiä tai poistaa olemassa olevia käyttäjiä Azure Active Directory (Azure AD)-organisaatiostasi:</span><span class="sxs-lookup"><span data-stu-id="71510-129">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="71510-130">Jos haluat lisätä uuden käyttäjän, Kirjaudu [Azure-portaaliin](https://ms.portal.azure.com/#home) organisaation käyttäjä järjestelmänvalvojana.</span><span class="sxs-lookup"><span data-stu-id="71510-130">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="71510-131">Valitse **Azure Active Directory**, valitse **käyttäjät** ja valitse sitten **Uusi käyttäjä**.</span><span class="sxs-lookup"><span data-stu-id="71510-131">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="71510-132">Täytä tarvittavat tiedot **käyttäjä** -sivulla.</span><span class="sxs-lookup"><span data-stu-id="71510-132">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="71510-133">Valitse **Luo**.</span><span class="sxs-lookup"><span data-stu-id="71510-133">Click **Create**.</span></span> <span data-ttu-id="71510-134">Käyttäjä luodaan ja lisätään Azure AD-vuokraajaan.</span><span class="sxs-lookup"><span data-stu-id="71510-134">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="71510-135">Lisä **tietoja**:</span><span class="sxs-lookup"><span data-stu-id="71510-135">**Learn more**:</span></span>

- [<span data-ttu-id="71510-136">Uuden käyttäjän lisääminen</span><span class="sxs-lookup"><span data-stu-id="71510-136">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="71510-137">Käyttäjän poistaminen</span><span class="sxs-lookup"><span data-stu-id="71510-137">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="71510-138">Käyttäjän profiili tietojen lisääminen tai päivittäminen Azure Active Directorya käyttäen</span><span class="sxs-lookup"><span data-stu-id="71510-138">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="71510-139">**Suositellut asia kirjat**</span><span class="sxs-lookup"><span data-stu-id="71510-139">**Recommended documents**</span></span>

- [<span data-ttu-id="71510-140">Mikä on roolipohjainen käytön hallinta (RBAC)?</span><span class="sxs-lookup"><span data-stu-id="71510-140">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="71510-141">Ymmärtämään eri rooleja Azuressa</span><span class="sxs-lookup"><span data-stu-id="71510-141">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="71510-142">Järjestelmänvalvojaroolin käyttö oikeudet Azure Active Directoryssa</span><span class="sxs-lookup"><span data-stu-id="71510-142">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="71510-143">Opetus ohjelma: käyttö oikeuksien myöntäminen käyttäjälle RBAC-ja Azure-portaalin avulla</span><span class="sxs-lookup"><span data-stu-id="71510-143">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="71510-144">RBAC-vian määritys Azuressa</span><span class="sxs-lookup"><span data-stu-id="71510-144">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="71510-145">Resurssien organisointi Azure Management Groupsin avulla</span><span class="sxs-lookup"><span data-stu-id="71510-145">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="71510-146">Azure-laskun kopion pyytäminen sähköpostitse</span><span class="sxs-lookup"><span data-stu-id="71510-146">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="71510-147">Luotto-tai maksu kortin lisääminen, päivittäminen tai poistaminen Azuresta</span><span class="sxs-lookup"><span data-stu-id="71510-147">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="71510-148">Tila uksen hallinta (Aktivoi uudelleen/Peruuta/Vaihda)</span><span class="sxs-lookup"><span data-stu-id="71510-148">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



