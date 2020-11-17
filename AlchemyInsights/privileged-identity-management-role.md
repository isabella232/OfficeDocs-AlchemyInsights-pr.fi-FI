---
title: Etuoikeutettu tunniste tietojen hallinta rooli
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088675"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="5f0a5-102">Etuoikeutettu tunniste tietojen hallinta (PIM)-rooli</span><span class="sxs-lookup"><span data-stu-id="5f0a5-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="5f0a5-103">**Käyttö oikeuksia ei myönnetä roolin Akti voinnin jälkeen**</span><span class="sxs-lookup"><span data-stu-id="5f0a5-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="5f0a5-104">Kun Akti voit roolin Azure AD etuoikeutettu käyttäjä tietojen hallinta (PIM)-ohjelmassa, Akti vointi ei välttämättä toimi välittömästi kaikissa portaaleista, jotka edellyttävät etuoikeutettua roolia.</span><span class="sxs-lookup"><span data-stu-id="5f0a5-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="5f0a5-105">Joskus, vaikka muutos olisi levitetty, verkko-väli muistiin tallentaminen portaalissa voi aiheuttaa sen, että muutos ei tule heti voimaan.</span><span class="sxs-lookup"><span data-stu-id="5f0a5-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="5f0a5-106">Jos Akti vointi viivästyy, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="5f0a5-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="5f0a5-107">Kirjaudu ulos Azure-portaalista ja kirjaudu sitten takaisin sisään.</span><span class="sxs-lookup"><span data-stu-id="5f0a5-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="5f0a5-108">Kun Akti voit Azure AD-roolin tai Azure-resurssi roolin, Akti voinnin vaiheet tulevat näkyviin.</span><span class="sxs-lookup"><span data-stu-id="5f0a5-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="5f0a5-109">Kun kaikki vaiheet on suoritettu, näkyviin tulee Kirjaudu ulos-linkki.</span><span class="sxs-lookup"><span data-stu-id="5f0a5-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="5f0a5-110">Tämän linkin avulla voit kirja utua ulos. Tämä ratkaisee useimmissa tapa uksissa aktivointi viiveen.</span><span class="sxs-lookup"><span data-stu-id="5f0a5-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="5f0a5-111">Varmista, että sinut on merkitty roolin jäseneksi PIM-ohjelmassa.</span><span class="sxs-lookup"><span data-stu-id="5f0a5-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="5f0a5-112">Jos Akti voit Exchange-järjestelmänvalvojaroolin, varmista, että kirja udut ulos ja kirja udut takaisin sisään.</span><span class="sxs-lookup"><span data-stu-id="5f0a5-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="5f0a5-113">Jos ongelma jatkuu, avaa tuki pyyntö ja nosta se ongelmaksi.</span><span class="sxs-lookup"><span data-stu-id="5f0a5-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="5f0a5-114">Jos käytät Exchange-järjestelmänvalvojien roolia tieto turva-ja yhteensopivuus keskuksen käyttämiseen, Katso seuraava vaihe.</span><span class="sxs-lookup"><span data-stu-id="5f0a5-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="5f0a5-115">Jos aktivoitan roolin tieto turva-ja yhteensopivuus keskuksen käyttöön tai Akti voit SharePoint-järjestelmänvalvojaroolin, Akti vointi viivästyy muutamasta minuutista muutamaan tuntiin.</span><span class="sxs-lookup"><span data-stu-id="5f0a5-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="5f0a5-116">Tämä on tunnettu ongelma, ja työskentelemme aktiivisesti näiden tiimien kanssa ongelman ratkaisemiseksi mahdollisimman pian.</span><span class="sxs-lookup"><span data-stu-id="5f0a5-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="5f0a5-117">Lisätietoja on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="5f0a5-117">For more information, see:</span></span>

- [<span data-ttu-id="5f0a5-118">Azure AD-roolien Akti voiminen PIM-ohjelmassa</span><span class="sxs-lookup"><span data-stu-id="5f0a5-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="5f0a5-119">Azure-resurssi roolien Akti voiminen PIM-ohjelmassa</span><span class="sxs-lookup"><span data-stu-id="5f0a5-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="5f0a5-120">**Käyttö oikeuksia ei poisteta sen jälkeen, kun rooli on poistettu käytöstä tai roolin Akti vointi on vanhentunut**</span><span class="sxs-lookup"><span data-stu-id="5f0a5-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="5f0a5-121">Kun poistat roolin käytöstä Azure AD:ssä, joka on etuoikeutettu käyttäjä tietojen hallinta tai kun roolin aktivointi aika päättyy, sinulla voi olla viive, jossa sinulla on edelleen käyttö oikeus.</span><span class="sxs-lookup"><span data-stu-id="5f0a5-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="5f0a5-122">Jos Akti voinnin poistaminen viivästyy, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="5f0a5-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="5f0a5-123">Jos poistat Exchange-järjestelmänvalvojaroolin Akti voinnin tai roolin aktivointi aika päättyy ja huomaat, että käyttö oikeudet ovat huomattavasti myöhässä, avaa tuki pyyntö ja pyydä tuki henkilön apua, jotta voit arkistoida lipun, jossa on Office-käyttö oikeuksien hallinnan (PAM) tiimi.</span><span class="sxs-lookup"><span data-stu-id="5f0a5-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="5f0a5-124">Jos aktivointi aika on vanhentunut, mutta selain istunto on edelleen avoinna, sulje selain.</span><span class="sxs-lookup"><span data-stu-id="5f0a5-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="5f0a5-125">Voit jatkaa roolin käyttöä, kunnes suljet istunnon.</span><span class="sxs-lookup"><span data-stu-id="5f0a5-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="5f0a5-126">Tämä on tunnettu ongelma, ja tarkastelemme mahdollisia korjauksia, joilla jokainen istunto peruutetaan aktiivisesti, kun Akti vointi on vanhentunut.</span><span class="sxs-lookup"><span data-stu-id="5f0a5-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="5f0a5-127">Jos viivästys ei ole sama kuin näissä kahdessa skenaariossa, avaa tuki pyyntö.</span><span class="sxs-lookup"><span data-stu-id="5f0a5-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
