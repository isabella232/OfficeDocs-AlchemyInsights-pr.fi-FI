---
title: MFA liittyvät ongelmat
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
ms.openlocfilehash: 2e79040c249b7825b964a19c51bcc42e5a6afb3f
ms.sourcegitcommit: 514ced512d0d7fff485b6fbf236cd27d6b4166e0
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/26/2019
ms.locfileid: "35250162"
---
# <a name="issues-with-mfa"></a><span data-ttu-id="c24fc-102">MFA liittyvät ongelmat</span><span class="sxs-lookup"><span data-stu-id="c24fc-102">Issues with MFA</span></span>
<span data-ttu-id="c24fc-103">On pari asiaa, jotka kannattaa tarkistaa, jos käyttäjiä ei voi kirjautua sisään käyttäen monitasoisen todennuksen (MFA)</span><span class="sxs-lookup"><span data-stu-id="c24fc-103">There are a couple of things to check if users cannot login using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="c24fc-104">Ongelman kohdanneen käyttäjän on ehkä estetty Azure Active Directory Portal.</span><span class="sxs-lookup"><span data-stu-id="c24fc-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="c24fc-105">Jos näin on, todennus yrittää kyseisen käyttäjän automaattisesti hylätään.</span><span class="sxs-lookup"><span data-stu-id="c24fc-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="c24fc-106">Noudata tämän artikkelin torjunnan purkamista.</span><span class="sxs-lookup"><span data-stu-id="c24fc-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="c24fc-107">Jos käyttäjän eston ollut apua tai ei ole estetty käyttäjä voi yrittää palauttaa käyttäjän MFA ja ne menevät läpi Rekisteröi uudelleen.</span><span class="sxs-lookup"><span data-stu-id="c24fc-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="c24fc-108">Noudattamalla tässä artikkelissa olevia ohjeita.</span><span class="sxs-lookup"><span data-stu-id="c24fc-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="c24fc-109">Jos tämä on ensimmäistä kertaa MFA käytössä ja käyttäjillä ei voi kirjautua sisään selaimet asiakkaita, kuten Outlook, Skype jne, ehkä ADAL (Active Directory Authentication kirjasto) ei ole käytössä tilauksesi O365.</span><span class="sxs-lookup"><span data-stu-id="c24fc-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="c24fc-110">Tässä tapauksessa sinun on Exchange Online-Powershell muodostaa yhteyden ja suorittaa tämä cmdlet-komento:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*</span><span class="sxs-lookup"><span data-stu-id="c24fc-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>