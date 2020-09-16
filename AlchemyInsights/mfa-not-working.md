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
# <a name="issues-with-azure-mfa"></a>Azure MFA-ongelmat
On muutamia asioita, jotka on tarkistettava, jos käyttäjät eivät voi kirja utua sisään monimenetelmäisen todentamisen avulla (MFA)

1. Haavoittuvuuden sisältävä käyttäjä on ehkä estynyt Azure Active Directory-portaalissa. Tässä tapa uksessa tietyn käyttäjän todennus yritykset kielletään automaattisesti. [Poista niiden esto noudattamalla tämän artikkelin ohjeita.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Jos käyttäjän eston poistaminen ei auttanut tai käyttäjää ei ole torjunut, voit yrittää palauttaa MFA-toiminnon käyttäjää varten, jolloin hän käy rekisteröinti prosessin läpi uudelleen. [Noudata tämän artikkelin ohjeita.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Jos tämä on ensimmäinen kerta, kun olet ottanut MFA:N käyttöön ja käyttäjät eivät voi kirja utua muihin kuin selaimiin, kuten Outlookiin, Skypeen, jne, ehkäpä ADAL (Active Directory-todennus kirjasto) ei ole käytössä O365-tila uksessa. Tässä tapa uksessa sinun on muodostettava yhteys Exchange Online PowerShelliin ja suoritettava tämä cmdlet-toiminto:  *asento-OrganizationConfig-OAuth2ClientProfileEnabled: $True*