---
title: Ongelman vian määritys-käyttäjää ei löydy hakemistosta
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 512494a69ab274af00962cb9777a3479b4200fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725404"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="0f2b0-102">Ongelman vian määritys-käyttäjää ei löydy hakemistosta</span><span class="sxs-lookup"><span data-stu-id="0f2b0-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="0f2b0-103">Jos käyttäjät saavat virhe ilmoituksen "käyttäjää ei löydy" hakemistosta, yritä uudelleen, kun ongelma tyyppi on käyttäjä, joka ei ole hakemistossa.</span><span class="sxs-lookup"><span data-stu-id="0f2b0-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="0f2b0-104">Voit suorittaa ongelman vian määrityksen suorittamalla seuraavat vaiheet.</span><span class="sxs-lookup"><span data-stu-id="0f2b0-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="0f2b0-105">Varmista, että sähkö posti kutsun hyväksynyt tili on sama tili, jota käytetään kirjautumiseen myöhemmin.</span><span class="sxs-lookup"><span data-stu-id="0f2b0-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="0f2b0-106">Varmista, että käyttäjä käyttää samaa tiliä, jotta voit hyväksyä kutsun ja kirja utua sivustoon.</span><span class="sxs-lookup"><span data-stu-id="0f2b0-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="0f2b0-107">Lisä tietoja on Ohje aiheessa Microsoft- [Tilin aliaksien hallinta </a> Microsoft 365-kirjautumisen hallintaa](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)varten.</span><span class="sxs-lookup"><span data-stu-id="0f2b0-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="0f2b0-108">Selaa jokaiseen sivustoon, jossa käyttäjä saa virhe ilmoituksen.</span><span class="sxs-lookup"><span data-stu-id="0f2b0-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="0f2b0-109">Lisää "/_layouts/15/People.aspx/membershipgroupid = 0" (lainaus merkkien sisällä) sivuston URL-osoitteen loppuun.</span><span class="sxs-lookup"><span data-stu-id="0f2b0-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="0f2b0-110">Esimerkki: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="0f2b0-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="0f2b0-111">Valitse käyttäjä luettelosta.</span><span class="sxs-lookup"><span data-stu-id="0f2b0-111">Select the user from the list.</span></span>

- <span data-ttu-id="0f2b0-112">Valitse valinta nauhasta **Poista käyttö oikeudet** .</span><span class="sxs-lookup"><span data-stu-id="0f2b0-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="0f2b0-113">Lisää käyttäjä takaisin ja Lähetä kutsu käyttäjälle uudelleen.</span><span class="sxs-lookup"><span data-stu-id="0f2b0-113">Add back the User and Resend the invite to the user.</span></span>

