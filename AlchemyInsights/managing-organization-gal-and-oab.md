---
title: Organisaation yleisen osoiteluettelon ja offline-osoitteiston hallitseminen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: a7142d68f0197aaca733766daf30fe8a46f13f9e
ms.sourcegitcommit: 8b50994a2979778ce8474ce83bd86b60e7d2cb2f
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/05/2020
ms.locfileid: "44022435"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="71281-102">Organisaation yleisen osoiteluettelon (GAL) ja offline-osoitteiston (OAB) hallitseminen</span><span class="sxs-lookup"><span data-stu-id="71281-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="71281-103">Yleinen osoiteluettelo (GAL, Global Address List) on luettelo organisaation sähköpostia käyttävistä kohteista (mikä tahansa vastaanottaja, joka voi vastaanottaa sähköpostia).</span><span class="sxs-lookup"><span data-stu-id="71281-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="71281-104">Jokaiselle organisaatiolle luodaan automaattisesti yksi GAL-luettelo.</span><span class="sxs-lookup"><span data-stu-id="71281-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="71281-105">Voit luoda ylimääräisiä GAL-luetteloita eri käyttäjille organisaation tai sijainnin mukaan, mutta yksittäinen käyttäjä voi tarkastella ja käyttää vain yhtä GAL-luetteloa kerrallaan.</span><span class="sxs-lookup"><span data-stu-id="71281-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="71281-106">Jotkin sähköpostiohjelmat, kuten Outlook ja Windows, lataavat GAL-luettelon offline-käyttöä varten.</span><span class="sxs-lookup"><span data-stu-id="71281-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="71281-107">Tätä kutsutaan offline-osoitteistoksi (OAB, Offline Address Book).</span><span class="sxs-lookup"><span data-stu-id="71281-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="71281-108">Exchange Onlinessa OAB-luettelo päivitetään vain kerran kahdeksassa tunnissa, minkä jälkeen asiakkaiden tulee ladata se paikallisen OAB-kopion päivittämiseksi.</span><span class="sxs-lookup"><span data-stu-id="71281-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="71281-109">Vastaanottajan muutosten tulee näkyä ensin GAL-luettelossa, jotta ne voivat myöhemmin näkyä OAB-luettelossa.</span><span class="sxs-lookup"><span data-stu-id="71281-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="71281-110">Seuraavassa on joitain yleisiä GAL- ja OAB-käytäntöjä:</span><span class="sxs-lookup"><span data-stu-id="71281-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="71281-111">Saatat useista syistä haluta, että jotkin kohteet piilotetaan GAL-luettelosta.</span><span class="sxs-lookup"><span data-stu-id="71281-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="71281-112">Saat lisätietoja artikkelista [Osoiteluettelon vastaanottajien piilottaminen](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="71281-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="71281-113">Jos haluat antaa tiettyjen käyttäjäryhmien tarkastella organisaation GAL-luettelon mukautettua näkymää, saat lisätietoja artikkelista [Osoitekirjakäytännöt Exchange Onlinessa](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="71281-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="71281-114">[Yleisen osoiteluettelon luominen Exchange Onlinessa](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list). Saat lisätietoja GAL-käyttöoikeuksista artikkelista [Osoiteluettelot Exchange Onlinessa](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span><span class="sxs-lookup"><span data-stu-id="71281-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="71281-115">Huomaa, että jos luot uusia GAL-luetteloita, haluat ehkä luoda myös uuden OAB-luettelon.</span><span class="sxs-lookup"><span data-stu-id="71281-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="71281-116">Saat lisätietoja artikkelista [Offline-osoitteisto ja käytännöt](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="71281-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
