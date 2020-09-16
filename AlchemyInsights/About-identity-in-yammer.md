---
title: Tietoja tunniste tiedoista Yammerissa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664167"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="4d832-102">Tietoja tunniste tiedoista Yammerissa</span><span class="sxs-lookup"><span data-stu-id="4d832-102">About identity in Yammer</span></span>

<span data-ttu-id="4d832-103">On suositeltavaa, että kaikki verkot seuraavat vaiheita, jotta identiteettiin liittyviä ongelmia voidaan välttää:</span><span class="sxs-lookup"><span data-stu-id="4d832-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="4d832-104">Pane täytäntöön Office 365-käyttäjä tiedot, kun Microsoft 365-tilit on luotu Azure AD:ssä, jotta kaikki käyttäjät voivat kirja utua sisään käyttämällä ensisijaisia Microsoft 365-tilejään.</span><span class="sxs-lookup"><span data-stu-id="4d832-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="4d832-105">Lisä tietoja on Ohje aiheessa [Office 365-käyttäjä tietojen määrittäminen Yammer-käyttäjille](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="4d832-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="4d832-106">Useiden Yammer-verkostojen kokoaminen.</span><span class="sxs-lookup"><span data-stu-id="4d832-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="4d832-107">Aiemmat Yammer-määritykset sallivat useiden Yammer-verkostojen yhteyden yhteen vuokraajaan.</span><span class="sxs-lookup"><span data-stu-id="4d832-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="4d832-108">Lisä tietoja on Ohje aiheessa [verkko siirto: usean Yammer-verkoston kokoaminen](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="4d832-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="4d832-109">Vaihtoehtoisesti voit pakottaa Yammerin käyttö oikeuden estämään käyttäjiä Yammerista, jos heillä ei ole käyttö oikeutta.</span><span class="sxs-lookup"><span data-stu-id="4d832-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="4d832-110">Lisä tietoja on Ohje aiheessa [Yammer-käyttö oikeuksien hallinta Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)-sovelluksessa.</span><span class="sxs-lookup"><span data-stu-id="4d832-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="4d832-111">Valvo lopuksi vanhojen Yammer-verkostojen käyttäjä luetteloa ja Keskeytä vanhat käyttäjät.</span><span class="sxs-lookup"><span data-stu-id="4d832-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="4d832-112">On suositeltavaa keskeyttää (poistaa käytöstä) käyttäjät niiden poistamisen sijaan, koska poisto on peruuttamaton.</span><span class="sxs-lookup"><span data-stu-id="4d832-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="4d832-113">Lisä tietoja on Ohje aiheessa [Yammer-käyttäjien valvonta Office 365-verkoissa](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) ja [käyttäjien poistaminen](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="4d832-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="4d832-114">Määrittämällä Yammerin näiden vaiheiden avulla voit myös määrittää Yammer-verkoston Microsoft 365-ohjelman alkuperäistä tilaa varten.</span><span class="sxs-lookup"><span data-stu-id="4d832-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="4d832-115">Lisä tietoja on Ohje aiheessa [Yammer-verkoston määrittäminen Microsoft 365-tila uksen alkuperäistä tilaa](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode)varten.</span><span class="sxs-lookup"><span data-stu-id="4d832-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>