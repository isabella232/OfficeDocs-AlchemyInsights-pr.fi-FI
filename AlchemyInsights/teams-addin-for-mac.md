---
title: Teams-apuohjelman lisääminen Maciin
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582067"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="fda79-102">Teams-apuohjelman lisääminen Maciin</span><span class="sxs-lookup"><span data-stu-id="fda79-102">Teams add-in for Mac</span></span>

<span data-ttu-id="fda79-103">Voit tehdä vianmäärityksen Teams-apuohjelman Mac-käyttöjärjestelmän käyttäjille seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="fda79-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="fda79-104">**Vaihe 1:** Jos käytössäsi on Exchange yhdistelmäympäristö (2016 CU3 tai uudempi), varmista Test-HMA.ps1-työkalun avulla, että moderni yhdistelmä varmennus on määritetty oikein.</span><span class="sxs-lookup"><span data-stu-id="fda79-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="fda79-105">Lisätietoja on kohdassa Modernin yhdistelmäympäristön [todentamisen määrityksen Outlook iOS- ja Android-versioille.](https://aka.ms/TestHMAEAS)</span><span class="sxs-lookup"><span data-stu-id="fda79-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="fda79-106">**Huomautus** Käytä UPN-osoitemuotoa (esimerkiksi [username@contoso.com](mailto:username@contoso.com)), älä toimialue\käyttäjänimi.</span><span class="sxs-lookup"><span data-stu-id="fda79-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="fda79-107">Voit tehdä tämän myös käyttäjille, joilla on Exchange Online postilaatikoita.</span><span class="sxs-lookup"><span data-stu-id="fda79-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="fda79-108">**Vaihe 2:** Käyttäjän täytyy valita **TyökalutTilit...**  >   ja Outlook for Mac ja etsi ja valitse tili.</span><span class="sxs-lookup"><span data-stu-id="fda79-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="fda79-109">Varmista, että käyttäjänimi on upn-muodossa (esimerkiksi [username@contoso.com).](mailto:username@contoso.com)</span><span class="sxs-lookup"><span data-stu-id="fda79-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="fda79-110">**Vaihe 3:** Varmista, että käyttäjällä on Microsoft Teams käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="fda79-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="fda79-111">Käyttäjän on käytettävä Office 365 for Mac -tilausta, tuoteversiota 16.24 tai uudempaa versiota.</span><span class="sxs-lookup"><span data-stu-id="fda79-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>