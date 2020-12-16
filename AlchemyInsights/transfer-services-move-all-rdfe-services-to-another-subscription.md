---
title: Siirto Palvelut – Siirrä kaikki RFE-Palvelut toiseen tila ukseen
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692042"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="b913e-102">Siirto Palvelut – Siirrä kaikki RFE-Palvelut toiseen tila ukseen</span><span class="sxs-lookup"><span data-stu-id="b913e-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="b913e-103">**Siirrä resursseja**</span><span class="sxs-lookup"><span data-stu-id="b913e-103">**Move resources**</span></span>

<span data-ttu-id="b913e-104">Azure-resurssit voidaan siirtää toiseen Azure-tila ukseen tai resurssi ryhmään saman tila uksen kautta käyttämällä Azure portaalia, Azure PowerShelliä, Azure CLI-liittymää tai REST-ohjelmointi raja pintaa resurssien siirtämiseen.</span><span class="sxs-lookup"><span data-stu-id="b913e-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="b913e-105">Ennen kuin voit siirtää resursseja, Katso:</span><span class="sxs-lookup"><span data-stu-id="b913e-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="b913e-106">Tarkistus luettelo ennen resurssien siirtämistä</span><span class="sxs-lookup"><span data-stu-id="b913e-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="b913e-107">Siirrettävät palvelut</span><span class="sxs-lookup"><span data-stu-id="b913e-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="b913e-108">Siirron vahvistaminen</span><span class="sxs-lookup"><span data-stu-id="b913e-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="b913e-109">Palveluiden ohjeiden siirtäminen</span><span class="sxs-lookup"><span data-stu-id="b913e-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="b913e-110">Jos haluat siirtää olemassa olevat resurssit toiseen resurssi ryhmään tai-tila ukseen, voit käyttää:</span><span class="sxs-lookup"><span data-stu-id="b913e-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="b913e-111">Azure-portaali</span><span class="sxs-lookup"><span data-stu-id="b913e-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="b913e-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="b913e-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="b913e-113">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="b913e-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="b913e-114">REST-OHJELMOINTI RAJA PINTA</span><span class="sxs-lookup"><span data-stu-id="b913e-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="b913e-115">Opetus ohjelma: [Azure-resurssien siirtäminen toiseen resurssi ryhmään tai-tila ukseen](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="b913e-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="b913e-116">**Virheiden vian määritys Azure Resource Managerilla**</span><span class="sxs-lookup"><span data-stu-id="b913e-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="b913e-117">Seuraavissa artikkeleissa on lisä tietoja joistakin yleisistä Azure-käyttöönotto virheistä ja niiden ratkaisemisesta.</span><span class="sxs-lookup"><span data-stu-id="b913e-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="b913e-118">Jos et löydä käyttöönotto virheesi virhe koodia, Katso lisä tietoja artikkelista [Virhe koodin](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)hakeminen.</span><span class="sxs-lookup"><span data-stu-id="b913e-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="b913e-119">Käyttöönotto virheiden vian määritys</span><span class="sxs-lookup"><span data-stu-id="b913e-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="b913e-120">Azure-resurssien siirtämiseen uuteen resurssi ryhmään tai-tila ukseen liittyviä ongelmia</span><span class="sxs-lookup"><span data-stu-id="b913e-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="b913e-121">Huomaa, että jos haluat päivittää Azure-pakettisi, kuten siirtymisestä maksuttomien maksu tietojen mukaan, sinun on muunnettava pakettisi.</span><span class="sxs-lookup"><span data-stu-id="b913e-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="b913e-122">Jos haluat päivittää maksuttomat kokeilu versiot, Katso lisä tietoja artikkelista [maksuttomien kokeilu versioiden päivittäminen tai Microsoft Imagine Azure-tilaus](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span><span class="sxs-lookup"><span data-stu-id="b913e-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="b913e-123">Jos haluat muuttaa pay-as-you-go-tiliä, Katso lisä tietoja artikkelista [Azure pay-as-you-go-tila uksen vaihtaminen eri tarjoukseen](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="b913e-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="b913e-124">**Azure-tila uksen lisääminen tai liittäminen Azure Active Directory-vuokraajaan:**</span><span class="sxs-lookup"><span data-stu-id="b913e-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="b913e-125">Kirjaudu sisään ja valitse tilaus, jota haluat käyttää [Azure-portaalin tila ukset-sivulla](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="b913e-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="b913e-126">Valitse **Vaihda hakemisto**.</span><span class="sxs-lookup"><span data-stu-id="b913e-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="b913e-127">Tarkista näkyviin tulevat varoitukset ja valitse sitten **Muuta**.</span><span class="sxs-lookup"><span data-stu-id="b913e-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="b913e-128">Tila uksen hakemistoa muutetaan ja saat Onnistumis viestin.</span><span class="sxs-lookup"><span data-stu-id="b913e-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="b913e-129">Siirry uuteen hakemistoon *hakemiston* valitsimen avulla.</span><span class="sxs-lookup"><span data-stu-id="b913e-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="b913e-130">Voi kestää jopa 10 minuuttia, ennen kuin kaikki näkyy oikein.</span><span class="sxs-lookup"><span data-stu-id="b913e-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="b913e-131">**Suositellut asia kirjat**</span><span class="sxs-lookup"><span data-stu-id="b913e-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="b913e-132">Azure-tila uksen omistajuuden siirtäminen</span><span class="sxs-lookup"><span data-stu-id="b913e-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="b913e-133">Resurssien siirtäminen uuteen resurssi ryhmään tai-tila ukseen</span><span class="sxs-lookup"><span data-stu-id="b913e-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="b913e-134">Resurssien hallinta Azure-portaalin avulla</span><span class="sxs-lookup"><span data-stu-id="b913e-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
