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
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/25/2019
ms.locfileid: "36545160"
---
# <a name="issues-with-mfa"></a>Makrotaloudellisen rahoitus avun ongelmat
On olemassa muutamia asioita tarkistaa, jos käyttäjät eivät voi kirja utua käyttäen Multi-Factor todennus (MFA)

1. Haavoittuvuuden saanut käyttäjä voidaan estää Azure Active Directory-portaalissa. Tällöin tietyn käyttäjän todennus yritykset estetään automaattisesti. [Voit poistaa eston noudattamalla tämän artikkelin ohjeita.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Jos eston käyttäjä ei auta tai käyttäjä ei ole estetty voit yrittää nollata MFA käyttäjälle ja he menevät läpi ilmoittautumisen prosessi uudelleen. [Noudata tämän artikkelin ohjeita.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Jos tämä on ensimmäinen kerta, kun otat MFA ja käyttäjät eivät voi kirja utua kuin selaimet asiakkaita, kuten Outlook, Skype jne, ehkä ADAL (Active Directory Authentication Library) ei ole käytössä O365 tilauksesi. Tässä tapa uksessa sinun täytyy muodostaa yhteys Exchange Online PowerShell ja suorita tämä cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*