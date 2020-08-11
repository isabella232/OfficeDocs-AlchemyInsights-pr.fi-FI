---
title: Teams-apuohjelma Macille
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/11/2020
ms.locfileid: "46629547"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="d351d-102">Teams-apuohjelma Macille</span><span class="sxs-lookup"><span data-stu-id="d351d-102">Teams add-in for Mac</span></span>

<span data-ttu-id="d351d-103">Jos haluat suorittaa puuttuvien teamsin apuohjelmien vian määrityksen Mac-käyttö järjestelmän käyttäjille, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="d351d-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="d351d-104">**Vaihe 1:** Jos sinulla on paikallisesti käytettävä yhdistelmä vaihto (2016 CU3 tai uudempi), varmista Test-HMA.ps1-työkalun avulla, että moderni yhdistelmä todennus on määritetty oikein.</span><span class="sxs-lookup"><span data-stu-id="d351d-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="d351d-105">Lisä tietoja on Ohje aiheessa [nykyaikaisen yhdistelmä ympäristön todennus määrityksen vahvistaminen Outlook for iOS:ssä ja Androidissa](https://aka.ms/AA980zq).</span><span class="sxs-lookup"><span data-stu-id="d351d-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="d351d-106">**Huomautus** Käytä UPN-osoite muotoa (esimerkiksi [username@contoso.com](mailto:username@contoso.com)), ei toimi alue \ käyttäjä nimi.</span><span class="sxs-lookup"><span data-stu-id="d351d-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="d351d-107">Tee näin myös käyttäjille, joilla on Exchange Online-posti laatikot.</span><span class="sxs-lookup"><span data-stu-id="d351d-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="d351d-108">**Vaihe 2:** Jos haluat, että käyttäjä siirtyy **Työkalut**-  >  **tiliin**... Outlook for Macissa ja Etsi ja valitse tili.</span><span class="sxs-lookup"><span data-stu-id="d351d-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="d351d-109">Varmista, että mainittu käyttäjä nimi on UPN-muodossa (esimerkiksi [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="d351d-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="d351d-110">**Vaihe 3:** Vahvista, että käyttäjä on lisensoitu Microsoft teams-käyttäjä.</span><span class="sxs-lookup"><span data-stu-id="d351d-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="d351d-111">Käyttäjällä on oltava käytössä Office 365 for Mac-tilaus, tuote versio 16,24 tai uudempi.</span><span class="sxs-lookup"><span data-stu-id="d351d-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>