---
title: MFA-ongelmat
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755128"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="8b3d7-102">Azure MFA-ongelmat</span><span class="sxs-lookup"><span data-stu-id="8b3d7-102">Issues with Azure MFA</span></span>
<span data-ttu-id="8b3d7-103">On muutamia asioita, jotka on tarkistettava, jos käyttäjät eivät voi kirja utua sisään monimenetelmäisen todentamisen avulla (MFA)</span><span class="sxs-lookup"><span data-stu-id="8b3d7-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="8b3d7-104">Haavoittuvuuden sisältävä käyttäjä on ehkä estynyt Azure Active Directory-portaalissa.</span><span class="sxs-lookup"><span data-stu-id="8b3d7-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="8b3d7-105">Tässä tapa uksessa tietyn käyttäjän todennus yritykset kielletään automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="8b3d7-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="8b3d7-106">Poista niiden esto noudattamalla tämän artikkelin ohjeita.</span><span class="sxs-lookup"><span data-stu-id="8b3d7-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="8b3d7-107">Jos käyttäjän eston poistaminen ei auttanut tai käyttäjää ei ole torjunut, voit yrittää palauttaa MFA-toiminnon käyttäjää varten, jolloin hän käy rekisteröinti prosessin läpi uudelleen.</span><span class="sxs-lookup"><span data-stu-id="8b3d7-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="8b3d7-108">Noudata tämän artikkelin ohjeita.</span><span class="sxs-lookup"><span data-stu-id="8b3d7-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="8b3d7-109">Jos tämä on ensimmäinen kerta, kun olet ottanut MFA:N käyttöön ja käyttäjät eivät voi kirja utua muihin kuin selaimiin, kuten Outlookiin, Skypeen, jne, ehkäpä ADAL (Active Directory-todennus kirjasto) ei ole käytössä O365-tila uksessa.</span><span class="sxs-lookup"><span data-stu-id="8b3d7-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="8b3d7-110">Tässä tapa uksessa sinun on muodostettava yhteys Exchange Online PowerShelliin ja suoritettava tämä cmdlet-toiminto:  *asento-OrganizationConfig-OAuth2ClientProfileEnabled: $True*</span><span class="sxs-lookup"><span data-stu-id="8b3d7-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>