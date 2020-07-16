---
title: Tietoja Yammerin käyttäjätiedoista
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148234"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="69309-102">Tietoja Yammerin käyttäjätiedoista</span><span class="sxs-lookup"><span data-stu-id="69309-102">About identity in Yammer</span></span>

<span data-ttu-id="69309-103">On suositeltavaa, että kaikki verkot ryhtyvät seuraaviin toimiin identiteettiin liittyvien ongelmien välttämiseksi:</span><span class="sxs-lookup"><span data-stu-id="69309-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="69309-104">Office 365 -käyttäjätietojen käyttäminen Sen jälkeen, kun Azure AD :n käyttäjät ovat varanneet Microsoft 365 -tilit, jotta kaikki käyttäjät kirjautuvat sisään käyttämällä ensisijaista Microsoft 365 -tiliä.</span><span class="sxs-lookup"><span data-stu-id="69309-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="69309-105">Lisätietoja on [ohjeaiheessa Office 365 -käyttäjätietojen käyttäminen Yammer-käyttäjille](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="69309-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="69309-106">Yhdistä useita Yammer-verkkoja.</span><span class="sxs-lookup"><span data-stu-id="69309-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="69309-107">Vanhat Yammer-määritykset sallivat useiden Yammer-verkkojen liittämisen yhteen vuokraajaan.</span><span class="sxs-lookup"><span data-stu-id="69309-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="69309-108">Lisätietoja on ohjeaiheessa [Verkon siirto - Useiden Yammer-verkkojen yhdistäminen](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="69309-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="69309-109">Voit halutessasi estää Yammerin käyttäjät Yammerista, jos heillä ei ole käyttöoikeutta.</span><span class="sxs-lookup"><span data-stu-id="69309-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="69309-110">Lisätietoja on [ohjeaiheessa Yammer-käyttöoikeuksien hallinta Office 365:ssä](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="69309-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="69309-111">Lopuksi, valvoa käyttäjäluettelo vanhempien Yammer-verkkojen ja keskeyttää vanhoja käyttäjiä.</span><span class="sxs-lookup"><span data-stu-id="69309-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="69309-112">On suositeltavaa keskeyttää (poistaa) käyttäjät (poistaa ne käytöstä) sen sijaan, että poistat ne, koska poisto on peruuttamatonta.</span><span class="sxs-lookup"><span data-stu-id="69309-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="69309-113">Lisätietoja on ohjeissa [Yammerin käyttäjien valvonta Office 365:ssä ja](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) [Käyttäjien poistaminen](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="69309-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="69309-114">Määrittämällä Yammerin näiden vaiheiden avulla voit myös määrittää Yammer-verkon Microsoft 365:n natiivitilaa varten.</span><span class="sxs-lookup"><span data-stu-id="69309-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="69309-115">Lisätietoja on [ohjeaiheessa Yammer-verkon määrittäminen Microsoft 365:n natiivitilaa varten](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="69309-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>