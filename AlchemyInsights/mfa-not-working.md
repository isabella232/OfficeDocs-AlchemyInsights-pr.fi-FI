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
ms.openlocfilehash: a415116b9ba437cb13426896119cd1b40d9ab491
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768834"
---
# <a name="issues-with-azure-mfa"></a>Azure MFA-ongelmat
On olemassa muutamia asioita, joilla voit tarkistaa, jos käyttäjät eivät voi kirja utua sisään käyttäen monimitostodennusta (MFA)

1. Haavoittuvuuden saanut käyttäjä voidaan estää Azure Active Directory-portaalissa. Tällöin tietyn käyttäjän todennus yritykset estetään automaattisesti. [Voit poistaa eston noudattamalla tämän artikkelin ohjeita.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Jos eston käyttäjä ei auta tai käyttäjä ei ole estetty voit yrittää nollata MFA käyttäjälle ja he menevät läpi ilmoittautumisen prosessi uudelleen. [Noudata tämän artikkelin ohjeita.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Jos tämä on ensimmäinen kerta, kun otat MFA ja käyttäjät eivät voi kirja utua kuin selaimet asiakkaita, kuten Outlook, Skype jne, ehkä ADAL (Active Directory Authentication Library) ei ole käytössä O365 tilauksesi. Tässä tapa uksessa sinun täytyy muodostaa yhteys Exchange Online PowerShell ja suorita tämä cmdlet:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $True*