---
title: Azure-laskutuksen omistajuuden siirtäminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922073"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="14c2b-102">Azure-laskutuksen omistajuuden siirtäminen</span><span class="sxs-lookup"><span data-stu-id="14c2b-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="14c2b-103">Kirjaudu sisään Azure- [portaaliin](https://portal.azure.com/) sen laskutus tilin järjestelmänvalvojana, jonka tila uksen haluat siirtää.</span><span class="sxs-lookup"><span data-stu-id="14c2b-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="14c2b-104">Jos et ole varma, onko olet järjestelmänvalvoja tai jos haluat selvittää, kuka on, Katso lisä tietoja artikkelista [tilin laskutuksen hallinnoijan määrittäminen](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="14c2b-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="14c2b-105">Etsi **kustannusten hallinta + laskutus**.</span><span class="sxs-lookup"><span data-stu-id="14c2b-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="14c2b-106">Valitse **paketteja** vasemmasta ruudusta.</span><span class="sxs-lookup"><span data-stu-id="14c2b-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="14c2b-107">Käyttö oikeuksien mukaan sinun on ehkä valittava laskutus alue ja sitten **tila uksia** tai **Azure-tila uksia**.</span><span class="sxs-lookup"><span data-stu-id="14c2b-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="14c2b-108">Valitse Siirrä **laskutuksen omistajuus** tilaukselle, jonka haluat siirtää.</span><span class="sxs-lookup"><span data-stu-id="14c2b-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="14c2b-109">Kirjoita sen käyttäjän Sähkö posti osoite, joka on sen tilin laskutuksen järjestelmänvalvoja, joka on uuden tila uksen omistaja ja valitse sitten **Lähetä siirto pyyntö**</span><span class="sxs-lookup"><span data-stu-id="14c2b-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="14c2b-110">Käyttäjä saa Sähkö posti viestin, jossa on ohjeet siirto pyynnön tarkistamiseen.</span><span class="sxs-lookup"><span data-stu-id="14c2b-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="14c2b-111">Jos haluat hyväksyä siirto pyynnön, käyttäjä valitsee Sähkö posti viestissä olevan linkin ja noudattaa annettuja ohjeita.</span><span class="sxs-lookup"><span data-stu-id="14c2b-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="14c2b-112">**Huomautus** : Jos siirrät tila uksen laskutuksen omistajuuden toisen Azure AD-vuokra ajan käyttäjän tiliin, Kaikki tila uksen resurssien hallintaan tarvittavat [Roolipohjaiset käyttö oikeuksien hallinta](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)tehtävät poistetaan pysyvästi.</span><span class="sxs-lookup"><span data-stu-id="14c2b-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="14c2b-113">Vain uudella omistajalla on oikeus hallita tila uksen resursseja.</span><span class="sxs-lookup"><span data-stu-id="14c2b-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="14c2b-114">Lisä tietoja on Ohje aiheessa [tila uksen siirtäminen käyttäjälle toisessa Azure AD-vuokra](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)ajassa.</span><span class="sxs-lookup"><span data-stu-id="14c2b-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="14c2b-115">**Suositellut asia kirjat**</span><span class="sxs-lookup"><span data-stu-id="14c2b-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="14c2b-116">Azure-tila uksen laskutuksen omistajuuden siirtäminen toiselle tilille</span><span class="sxs-lookup"><span data-stu-id="14c2b-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="14c2b-117">Tietoja siitä, miten laskutus omistajuus siirretään Azure-tila ukseen</span><span class="sxs-lookup"><span data-stu-id="14c2b-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="14c2b-118">Visual Studion, Microsoft-partneri verkoston (MPN) siirtäminen ja maksu tapa-ja kokeilu tilaukset</span><span class="sxs-lookup"><span data-stu-id="14c2b-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="14c2b-119">Siirrä omistajuuden usein kysytyt kysymykset</span><span class="sxs-lookup"><span data-stu-id="14c2b-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="14c2b-120">Siirron omistus ongelmien vian määritys</span><span class="sxs-lookup"><span data-stu-id="14c2b-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
