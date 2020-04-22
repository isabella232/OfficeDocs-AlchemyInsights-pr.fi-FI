---
title: Ongelman vianmääritys - Käyttäjää ei löydy hakemistosta
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 3b863c5e9962dd29ca2ed41d113041d74830f615
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43702735"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a><span data-ttu-id="908f3-102">Ongelman vianmääritys - Käyttäjää ei löydy hakemistosta</span><span class="sxs-lookup"><span data-stu-id="908f3-102">Troubleshoot issue - User not found in directory</span></span>

<span data-ttu-id="908f3-103">Jos käyttäjät saavat hakemistosta virhesanoman "käyttäjää ei löydy", yritä uudelleen, missä seurantakohteen tyyppi ei ole hakemistossa.</span><span class="sxs-lookup"><span data-stu-id="908f3-103">If users are receiving error message "user can't be found" in the directory, please try again where the Issue Type is User not in directory.</span></span>

<span data-ttu-id="908f3-104">Seuraavat vaiheet voidaan suorittaa ongelman vianmäärityksen jälkeen.</span><span class="sxs-lookup"><span data-stu-id="908f3-104">The following steps can be completed to troubleshoot the issue.</span></span>

- <span data-ttu-id="908f3-105">Varmista, että sähköpostikutsun hyväksynyt tili on sama tili, jota käytetään myöhemmin kirjautumiseen.</span><span class="sxs-lookup"><span data-stu-id="908f3-105">Ensure the account that accepted the email invitation is the same account that is being used to sign in later.</span></span> <span data-ttu-id="908f3-106">Varmista, että käyttäjä käyttää samaa tiliä kutsuan hyväksymiseen ja kirjautumiseen sivustoon.</span><span class="sxs-lookup"><span data-stu-id="908f3-106">Make sure the user is using the same account to accept the invite and sign into the site.</span></span> 

<span data-ttu-id="908f3-107">Lisätietoja on [ohjeaiheessa Microsoft-tilin</a> aliasten hallinta Microsoft 365 -kirjautumisen hallintaa varten](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span><span class="sxs-lookup"><span data-stu-id="908f3-107">For more info, see [How to manage aliases for your Microsoft account</a> to manage the Microsoft 365 login](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases).</span></span> 

- <span data-ttu-id="908f3-108">Selaa jokaiseen sivustoon tai sivustoihin, joissa käyttäjä saa virheen.</span><span class="sxs-lookup"><span data-stu-id="908f3-108">Browse to each site(s) in which the user is receiving the error.</span></span> 

<span data-ttu-id="908f3-109">Lisää sivuston URL-osoitteen loppuun "/_layouts/15/people.aspx/membershipgroupid=0" (lainausmerkkien sisällä).</span><span class="sxs-lookup"><span data-stu-id="908f3-109">Add "/_layouts/15/people.aspx/membershipgroupid=0" (within the double-quotes) to the end of the site URL.</span></span> 

<span data-ttu-id="908f3-110">Esimerkki: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span><span class="sxs-lookup"><span data-stu-id="908f3-110">Example: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0.</span></span>

- <span data-ttu-id="908f3-111">Valitse käyttäjä luettelosta.</span><span class="sxs-lookup"><span data-stu-id="908f3-111">Select the user from the list.</span></span>

- <span data-ttu-id="908f3-112">Valitse valintanauhasta **Poista käyttöoikeudet.**</span><span class="sxs-lookup"><span data-stu-id="908f3-112">Click **Remove User Permissions** from the Ribbon.</span></span> 
-  <span data-ttu-id="908f3-113">Lisää käyttäjä takaisin ja Lähetä kutsu uudelleen käyttäjälle.</span><span class="sxs-lookup"><span data-stu-id="908f3-113">Add back the User and Resend the invite to the user.</span></span>

