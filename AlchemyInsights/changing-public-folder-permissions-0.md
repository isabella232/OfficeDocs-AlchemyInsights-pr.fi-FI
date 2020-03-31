---
title: Yleisen kansion käyttöoikeuksien muuttaminen
ms.author: dmaguire
author: msdmaguire
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "633"
- "3500007"
ms.assetid: 0c37ab75-c81c-44e7-bda8-ea43263f9fdf
ms.openlocfilehash: 68aefd820c681a9022828f67655e1c843692a30e
ms.sourcegitcommit: 92e9a649532f5231ceedcafc4d14b8ad18d517c2
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/31/2020
ms.locfileid: "43059769"
---
# <a name="changing-public-folder-permissions"></a><span data-ttu-id="0e53e-102">Yleisen kansion käyttöoikeuksien muuttaminen</span><span class="sxs-lookup"><span data-stu-id="0e53e-102">Changing public folder permissions</span></span>

<span data-ttu-id="0e53e-103">Outlookin käyttäjät ja järjestelmänvalvojat voivat muuttaa yleisen kansion käyttöoikeuksia.</span><span class="sxs-lookup"><span data-stu-id="0e53e-103">Public folder permissions can be changed by users and administrators in Outlook.</span></span> <span data-ttu-id="0e53e-104">Järjestelmänvalvojat voivat myös hallita Exchange Admin Centerin (EAC) käyttöoikeuksia seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="0e53e-104">Administrators can also control permissions from the Exchange Admin Center (EAC), by doing the following:</span></span>
  
1. <span data-ttu-id="0e53e-105">Siirry Microsoft 365 -hallintakeskuksessa **Kohtaan Hallintakeskukset** \> **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="0e53e-105">In the Microsoft 365 admin center, go to **Admin centers** \> **Exchange**.</span></span>

2. <span data-ttu-id="0e53e-106">Valitse **Julkiset kansiot**.</span><span class="sxs-lookup"><span data-stu-id="0e53e-106">Select **Public folders**.</span></span>

3. <span data-ttu-id="0e53e-107">Sieltä voit muuttaa yksittäisten yleisten kansioiden käyttöoikeuksia määrittämällä käyttöoikeusryhmille suojausryhmiä.</span><span class="sxs-lookup"><span data-stu-id="0e53e-107">From there, you can change permissions for individual public folders by assigning security groups to permissions.</span></span> <span data-ttu-id="0e53e-108">Jotta käyttäjä voi muuttaa yleisen kansion käyttöoikeuksia, käyttäjällä on oltava kansion omistajaoikeudet.</span><span class="sxs-lookup"><span data-stu-id="0e53e-108">For an end user to change public folder permissions, the user needs to have Owner rights on the folder.</span></span>

<span data-ttu-id="0e53e-109">Noudata ohjeita, jotka on kuvattu ohjeaiheessa [Yleisen kansion käyttöoikeusongelmien vianmääritys ja yleisen kansion käyttöoikeusongelmien vianmääritys.](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues)</span><span class="sxs-lookup"><span data-stu-id="0e53e-109">Please follow the procedure described in [How to diagnose and fix public folder permission issues](https://docs.microsoft.com/exchange/troubleshoot/public-folders/public-folder-permission-issues) to troubleshoot public folder permission issues.</span></span>

<span data-ttu-id="0e53e-110">**Huomautus**: Voit kohdata useita tunnettuja ongelmia, kun yrität muuttaa yleisten kansioiden käyttöoikeuksia.</span><span class="sxs-lookup"><span data-stu-id="0e53e-110">**Note**: There are several known issues you might encounter when you try to change permissions on public folders.</span></span> <span data-ttu-id="0e53e-111">Lisätietoja on seuraavissa artikkeleissa.</span><span class="sxs-lookup"><span data-stu-id="0e53e-111">See the following articles for more information.</span></span>

- [<span data-ttu-id="0e53e-112">Käyttöoikeuksia ei voi käyttää EAC:n yleisten kansioiden alikansioihin</span><span class="sxs-lookup"><span data-stu-id="0e53e-112">Can't apply permissions to public folder subfolders in EAC</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/can%E2%80%99t-apply-permissions-public-folder-subfolders)

- [<span data-ttu-id="0e53e-113">Postilaatikkoa ei löydy paikallisesta puuryhmästä -virhe käytettäessä yleisiä kansioita (tämä artikkeli on oikeatasoinen)</span><span class="sxs-lookup"><span data-stu-id="0e53e-113">"The mailbox is not found in the local forest" error when you access public folders</span></span>](https://docs.microsoft.com/exchange/troubleshoot/public-folders/mailbox-not-found-local-forest-public-folder)
