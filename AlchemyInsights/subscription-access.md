---
title: Tila uksen käyttäminen
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807431"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="c6cee-102">Kirjautuminen ei onnistu selaimen ongelmien vuoksi (selain jumittuu, pitää pyöriä, ei lataudu, jne.)</span><span class="sxs-lookup"><span data-stu-id="c6cee-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="c6cee-103">Sinulla voi olla katkos.</span><span class="sxs-lookup"><span data-stu-id="c6cee-103">You might be impacted by an outage.</span></span> <span data-ttu-id="c6cee-104">Tarkista, onko käytössä jatkuva katkos: [Azure Health-tila](https://status.azure.com/status/history/).</span><span class="sxs-lookup"><span data-stu-id="c6cee-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="c6cee-105">Kirjaudu ulos kaikista Active Azure-istunnoista.</span><span class="sxs-lookup"><span data-stu-id="c6cee-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="c6cee-106">Aloita selaimen yksityinen tai incognito-tila.</span><span class="sxs-lookup"><span data-stu-id="c6cee-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="c6cee-107">Voit myös yrittää päivittää selainta, käyttää toista selainta, poistaa väli muisti eväs teet, jos edellä ei toimi.</span><span class="sxs-lookup"><span data-stu-id="c6cee-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="c6cee-108">Lisä tietoja: [kirjautumisongelmien vian määritys](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="c6cee-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="c6cee-109">**Paketteja ei voi käyttää**</span><span class="sxs-lookup"><span data-stu-id="c6cee-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="c6cee-110">Varmista [Azure-portaalissa](https://portal.azure.com/), että oikea Azure-hakemisto on valittuna tilin oikeassa yläkulmassa.</span><span class="sxs-lookup"><span data-stu-id="c6cee-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="c6cee-111">Varmista [Azuren tili keskuksessa](https://account.windowsazure.com/Subscriptions), onko tili käytössä tilin järjestelmänvalvoja.</span><span class="sxs-lookup"><span data-stu-id="c6cee-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="c6cee-112">Lisä tietoja: [ei löydettyjä paketteja ei löydy](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="c6cee-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="c6cee-113">**Laskutus historiaa ei voi käyttää**</span><span class="sxs-lookup"><span data-stu-id="c6cee-113">**Unable to access billing history**</span></span>

<span data-ttu-id="c6cee-114">Tilin järjestelmänvalvojan on varmistettava, että laskutus tiedot sisältävä käyttäjä lisätään Azure Active Directoryyn vieras käyttäjänä: [uuden käyttäjän lisääminen tai poistaminen](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="c6cee-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="c6cee-115">Käyttäjälle on annettava yleinen järjestelmänvalvojan rooli: [roolin määrittäminen käyttäjille](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="c6cee-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="c6cee-116">Lähetä tämä käyttäjä voi antaa laskutukseen pääsyn RBAC-käytäntöjen avulla: [Myönnä käyttö oikeudet laskutukseen](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="c6cee-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="c6cee-117">**Suositellut asia kirjat**</span><span class="sxs-lookup"><span data-stu-id="c6cee-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="c6cee-118">En pysty Kirjautu maan Azure-tila uksen hallintaan</span><span class="sxs-lookup"><span data-stu-id="c6cee-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)