---
title: Ongelman vian määritys-käyttäjää ei löydy hakemistosta
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 59713231da25be441e7c05d788337e66bf17265a
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768798"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="6f023-102">Ongelman vian määritys-käyttäjää ei löydy hakemistosta</span><span class="sxs-lookup"><span data-stu-id="6f023-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="6f023-103">Jos käyttäjät saavat virhe sanoman "käyttäjää ei löydy" hakemistosta, yritä uudelleen, jos ongelma tyyppi on käyttäjä ei ole hakemistoon.</span><span class="sxs-lookup"><span data-stu-id="6f023-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="6f023-104">Seuraavat vaiheet voidaan suorittaa ongelman vian määritystä varten.</span><span class="sxs-lookup"><span data-stu-id="6f023-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="6f023-105">Varmista, että sähkö posti kutsun hyväksynyt tili on sama tili, jota käytetään kirjautumiseen myöhemmin.</span><span class="sxs-lookup"><span data-stu-id="6f023-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="6f023-106">Varmista, että käyttäjä käyttää samaa tiliä hyväksyäksesi kutsun ja kirjautumiseen sivustoon.</span><span class="sxs-lookup"><span data-stu-id="6f023-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="6f023-107">Lisä tietoja on Ohje aiheessa [Microsoft-tilin</a> tunnusten hallinta Office 365-kirjautumistietojen hallintaa](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)varten.</span><span class="sxs-lookup"><span data-stu-id="6f023-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Office 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="6f023-108">Selaa jokaiseen sivustoon, jossa käyttäjä saa virheen.</span><span class="sxs-lookup"><span data-stu-id="6f023-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="6f023-109">Lisää "/_layouts/15/People.aspx/membershipgroupid = 0" (lainaus merkkien sisällä) sivuston URL-osoitteen loppuun.</span><span class="sxs-lookup"><span data-stu-id="6f023-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="6f023-110">Esimerkki: https://< "contoso" >. sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="6f023-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="6f023-111">Valitse käyttäjä luettelosta.</span><span class="sxs-lookup"><span data-stu-id="6f023-111">Select the user from the list.</span></span>

- <span data-ttu-id="6f023-112">Valitse **Poista käyttö oikeudet** valinta nauhasta.</span><span class="sxs-lookup"><span data-stu-id="6f023-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="6f023-113">Lisää käyttäjä takaisin ja Lähetä kutsu käyttäjälle uudelleen.</span><span class="sxs-lookup"><span data-stu-id="6f023-113">Add back the User and Resend the invite to the user.</span></span>

