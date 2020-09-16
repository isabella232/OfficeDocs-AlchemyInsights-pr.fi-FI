---
title: Teams-apuohjelma Macille
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
- "9003233"
ms.openlocfilehash: 1e5f6d66386398ad8600f9383f9f7a1dcf0ce69f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670325"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="29f31-102">Teams-apuohjelma Macille</span><span class="sxs-lookup"><span data-stu-id="29f31-102">Teams add-in for Mac</span></span>

<span data-ttu-id="29f31-103">Jos haluat suorittaa puuttuvien teamsin apuohjelmien vian määrityksen Mac-käyttö järjestelmän käyttäjille, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="29f31-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="29f31-104">**Vaihe 1:** Jos sinulla on paikallisesti käytettävä yhdistelmä vaihto (2016 CU3 tai uudempi), varmista Test-HMA.ps1-työkalun avulla, että moderni yhdistelmä todennus on määritetty oikein.</span><span class="sxs-lookup"><span data-stu-id="29f31-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="29f31-105">Lisä tietoja on Ohje aiheessa [nykyaikaisen yhdistelmä ympäristön todennus määrityksen vahvistaminen Outlook for iOS:ssä ja Androidissa](https://aka.ms/AA980zq).</span><span class="sxs-lookup"><span data-stu-id="29f31-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="29f31-106">**Huomautus** Käytä UPN-osoite muotoa (esimerkiksi [username@contoso.com](mailto:username@contoso.com)), ei toimi alue \ käyttäjä nimi.</span><span class="sxs-lookup"><span data-stu-id="29f31-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="29f31-107">Tee näin myös käyttäjille, joilla on Exchange Online-posti laatikot.</span><span class="sxs-lookup"><span data-stu-id="29f31-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="29f31-108">**Vaihe 2:** Jos haluat, että käyttäjä siirtyy **Työkalut**-  >  **tiliin**... Outlook for Macissa ja Etsi ja valitse tili.</span><span class="sxs-lookup"><span data-stu-id="29f31-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="29f31-109">Varmista, että mainittu käyttäjä nimi on UPN-muodossa (esimerkiksi [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="29f31-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="29f31-110">**Vaihe 3:** Vahvista, että käyttäjä on lisensoitu Microsoft teams-käyttäjä.</span><span class="sxs-lookup"><span data-stu-id="29f31-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="29f31-111">Käyttäjällä on oltava käytössä Office 365 for Mac-tilaus, tuote versio 16,24 tai uudempi.</span><span class="sxs-lookup"><span data-stu-id="29f31-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>