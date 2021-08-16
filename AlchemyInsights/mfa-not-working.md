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
ms.openlocfilehash: b39c79063c66ea41585c8f9eec372bfac77bc0aa29ded5a5572e06c141b28f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54098599"
---
# <a name="issues-with-azure-mfa"></a>Azuren MFA-ongelmat
On muutamia asioita, jotka on hyvä tarkistaa, eivätkö käyttäjät voi kirjautua monimenetelmäisen todentamisen (MFA) avulla

1. Käyttäjä, jota ongelma koskee, on ehkä estetty Azure Active Directory portaalissa. Jos näin on, todennus yrittää tätä tiettyä käyttäjää varten automaattisesti. [Voit poistaa eston tämän artikkelin ohjeiden mukaisesti.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Jos käyttäjän eston poistaminen ei auta tai käyttäjää ei ole estetty, voit yrittää palauttaa käyttäjän MFA-sertifikaatit ja hän käy rekisteröintiprosessin läpi uudelleen. [Noudata tämän artikkelin ohjeita.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Jos tämä on ensimmäinen kerta, kun olet ottanut MFA:n käyttöön ja käyttäjäsi eivät voi kirjautua sisään ei-selaimissa, kuten Outlook-, Skype-, jne., ehkä ADAL:n (Active Directory -todennuskirjasto) ei ole käytössä O365 -tilauksessasi. Tässä tapauksessa sinun täytyy muodostaa yhteys Exchange Online Powershelliin ja suorittaa tämä cmdlet-komento: *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*