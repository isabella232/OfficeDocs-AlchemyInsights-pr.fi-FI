---
title: MFA-ongelmat
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810481"
---
# <a name="issues-with-azure-mfa"></a><span data-ttu-id="5c71f-102">Azuren MFA-ongelmat</span><span class="sxs-lookup"><span data-stu-id="5c71f-102">Issues with Azure MFA</span></span>
<span data-ttu-id="5c71f-103">On muutamia asioita, jotka on hyvä tarkistaa, eivätkö käyttäjät voi kirjautua monimenetelmäisen todentamisen (MFA) avulla</span><span class="sxs-lookup"><span data-stu-id="5c71f-103">There are a couple of things to check if users cannot log in using multi-factor authentication (MFA)</span></span>

1. <span data-ttu-id="5c71f-104">Käyttäjä, jota ongelma koskee, on ehkä estetty Azure Active Directory -portaalissa.</span><span class="sxs-lookup"><span data-stu-id="5c71f-104">The affected user may be blocked in Azure Active Directory Portal.</span></span> <span data-ttu-id="5c71f-105">Jos näin on, todennus yrittää tätä tiettyä käyttäjää varten automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="5c71f-105">If that is the case, Authentication attempts for that specific user will be automatically denied.</span></span> [<span data-ttu-id="5c71f-106">Voit poistaa eston tämän artikkelin ohjeiden mukaisesti.</span><span class="sxs-lookup"><span data-stu-id="5c71f-106">Please follow the steps in this article to unblock them.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. <span data-ttu-id="5c71f-107">Jos käyttäjän eston poistaminen ei auta tai käyttäjää ei ole estetty, voit yrittää palauttaa käyttäjän MFA-sertifikaatit ja hän käy rekisteröintiprosessin läpi uudelleen.</span><span class="sxs-lookup"><span data-stu-id="5c71f-107">If unblocking the user didn't help or the user is not blocked you can try to reset MFA for the user and they will go through the enroll process again.</span></span> [<span data-ttu-id="5c71f-108">Noudata tämän artikkelin ohjeita.</span><span class="sxs-lookup"><span data-stu-id="5c71f-108">Please follow the steps in this article.</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

<span data-ttu-id="5c71f-109">Jos tämä on ensimmäinen kerta, kun olet ottanut MFA:n käyttöön ja käyttäjäsi eivät voi kirjautua sisään ei-selaimiin, kuten Outlookiin, Skypeen jne., ehkä ADAL:iin (Active Directory -todentamiskirjasto) ei ole käytössä O365 -tilauksessasi.</span><span class="sxs-lookup"><span data-stu-id="5c71f-109">If this is the first time you enabled MFA and your users are unable to login to non-browsers clients such as Outlook, Skype, etc, perhaps ADAL (Active Directory Authentication Library) is not enabled on your O365 subscription.</span></span> <span data-ttu-id="5c71f-110">Tässä tapauksessa sinun täytyy muodostaa yhteys Exchange Online Powershelliin ja suorittaa tämä cmdlet-komento:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span><span class="sxs-lookup"><span data-stu-id="5c71f-110">In this case you will need to connect to Exchange Online Powershell and run this cmdlet:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*</span></span>