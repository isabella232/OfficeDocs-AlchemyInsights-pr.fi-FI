---
title: Vianmääritys ongelma - käyttäjän kansiota ei löydy
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 537b27d06acd17cbb3fe99bcb89e153099e92bb4
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36544860"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="904b7-102">Vianmääritys ongelma - käyttäjän kansiota ei löydy</span><span class="sxs-lookup"><span data-stu-id="904b7-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="904b7-103">Jos käyttäjät saavat virhe sanoma ”käyttäjää ei löydy-hakemistossa.</span><span class="sxs-lookup"><span data-stu-id="904b7-103">If users are receiving error message "user can't be found" in the directory.</span></span> <span data-ttu-id="904b7-104">Yritä uudelleen Jos seurantakohteen tyyppi ei käyttäjä kansio.</span><span class="sxs-lookup"><span data-stu-id="904b7-104">Please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="904b7-105">Seuraavat vaiheet voi suorittaa ongelman vianmäärityksen.</span><span class="sxs-lookup"><span data-stu-id="904b7-105">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="904b7-106">Varmista tilin, email-kutsu on sama tili, jota käytetään Jos haluat kirjautua sisään myöhemmin.</span><span class="sxs-lookup"><span data-stu-id="904b7-106">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="904b7-107">Varmista, että käyttäjä käyttää samaa tiliä, Kirjaudu sivustoon ja hyväksy kutsu.</span><span class="sxs-lookup"><span data-stu-id="904b7-107">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="904b7-108">Lisätietoja, katso [hallinnasta Microsoft-tilin aliaksia</a> voit hallita Office 365-kirjautumisen](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="904b7-108">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="904b7-109">Selaa kunkin teillä, jossa käyttäjä vastaanottaa virheen.</span><span class="sxs-lookup"><span data-stu-id="904b7-109">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="904b7-110">Lisää ”/ _layouts/15/people.aspx/membershipgroupid=0” (sisällä lainausmerkit) sivuston URL-Osoitteen loppuun.</span><span class="sxs-lookup"><span data-stu-id="904b7-110">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="904b7-111">Esimerkki: https://_lT _"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="904b7-111">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="904b7-112">Valitse käyttäjä luettelosta.</span><span class="sxs-lookup"><span data-stu-id="904b7-112">Select the user from the list.</span></span>

- <span data-ttu-id="904b7-113">Valitse valintanauhasta **poistaa käyttöoikeuksia** .</span><span class="sxs-lookup"><span data-stu-id="904b7-113">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="904b7-114">Lisää edellinen käyttäjä ja Lähetä kutsu käyttäjä.</span><span class="sxs-lookup"><span data-stu-id="904b7-114">Add back the User and Resend the invite to the user.</span></span>

