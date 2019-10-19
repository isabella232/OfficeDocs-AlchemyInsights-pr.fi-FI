---
title: Makrotaloudellisen rahoitus avun ongelmat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36545160"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="26149-102">Makrotaloudellisen rahoitus avun ongelmat</span><span class="sxs-lookup"><span data-stu-id="26149-102">Issues with MFA</span></span>
<span data-ttu-id="26149-103">On olemassa muutamia asioita tarkistaa, jos käyttäjät eivät voi kirja utua käyttäen Multi-Factor todennus (MFA)</span><span class="sxs-lookup"><span data-stu-id="26149-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="26149-104">Haavoittuvuuden saanut käyttäjä voidaan estää Azure Active Directory-portaalissa.</span><span class="sxs-lookup"><span data-stu-id="26149-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="26149-105">Tällöin tietyn käyttäjän todennus yritykset estetään automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="26149-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="26149-106">Voit poistaa eston noudattamalla tämän artikkelin ohjeita.</span><span class="sxs-lookup"><span data-stu-id="26149-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="26149-107">Jos eston käyttäjä ei auta tai käyttäjä ei ole estetty voit yrittää nollata MFA käyttäjälle ja he menevät läpi ilmoittautumisen prosessi uudelleen.</span><span class="sxs-lookup"><span data-stu-id="26149-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="26149-108">Noudata tämän artikkelin ohjeita.</span><span class="sxs-lookup"><span data-stu-id="26149-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="26149-109">Jos tämä on ensimmäinen kerta, kun otat MFA ja käyttäjät eivät voi kirja utua kuin selaimet asiakkaita, kuten Outlook, Skype jne, ehkä ADAL (Active Directory Authentication Library) ei ole käytössä O365 tilauksesi.</span><span class="sxs-lookup"><span data-stu-id="26149-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="26149-110">Tässä tapa uksessa sinun täytyy muodostaa yhteys Exchange Online PowerShell ja suorita tämä cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="26149-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>