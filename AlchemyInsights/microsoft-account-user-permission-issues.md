---
title: Luoda ja käyttää jaetun postilaatikon
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81bf8082198de1c44037291f23c434d06a77f02a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34762398"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="4ac7b-102">Vianmääritys ongelma - käyttäjän kansiota ei löydy</span><span class="sxs-lookup"><span data-stu-id="4ac7b-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="4ac7b-103">Jos käyttäjät saavat virhe sanoma ”käyttäjää ei löydy-hakemistossa.</span><span class="sxs-lookup"><span data-stu-id="4ac7b-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="4ac7b-104">Yritä uudelleen Jos seurantakohteen tyyppi ei käyttäjä kansio.</span><span class="sxs-lookup"><span data-stu-id="4ac7b-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="4ac7b-105">Seuraavat vaiheet voi suorittaa ongelman vianmäärityksen.</span><span class="sxs-lookup"><span data-stu-id="4ac7b-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="4ac7b-106">Varmista tilin, email-kutsu on sama tili, jota käytetään Jos haluat kirjautua sisään myöhemmin.</span><span class="sxs-lookup"><span data-stu-id="4ac7b-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="4ac7b-107">Varmista, että käyttäjä käyttää samaa tiliä, Kirjaudu sivustoon ja hyväksy kutsu.</span><span class="sxs-lookup"><span data-stu-id="4ac7b-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="4ac7b-108">Lisätietoja, katso [hallinnasta Microsoft-tilin aliaksia</a> voit hallita Office 365-kirjautumisen](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="4ac7b-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="4ac7b-109">Selaa kunkin teillä, jossa käyttäjä vastaanottaa virheen.</span><span class="sxs-lookup"><span data-stu-id="4ac7b-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="4ac7b-110">Lisää ”/ _layouts/15/people.aspx/membershipgroupid=0” (sisällä lainausmerkit) sivuston URL-Osoitteen loppuun.</span><span class="sxs-lookup"><span data-stu-id="4ac7b-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="4ac7b-111">Esimerkki: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="4ac7b-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="4ac7b-112">Valitse käyttäjä luettelosta.</span><span class="sxs-lookup"><span data-stu-id="4ac7b-112">Select the user from the list.</span></span>

- <span data-ttu-id="4ac7b-113">Valitse valintanauhasta **poistaa käyttöoikeuksia** .</span><span class="sxs-lookup"><span data-stu-id="4ac7b-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="4ac7b-114">Lisää edellinen käyttäjä ja Lähetä kutsu käyttäjä.</span><span class="sxs-lookup"><span data-stu-id="4ac7b-114">Add back the User and Resend the invite to the user.</span></span>

