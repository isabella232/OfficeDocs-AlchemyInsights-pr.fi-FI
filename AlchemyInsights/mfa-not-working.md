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
ms.openlocfilehash: 276f6b2212c9d85df726cb46a46dee7828b34c89
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36545160"
---
# <a name="issues-with-mfa"></a>MFA liittyvät ongelmat
On pari asiaa, jotka kannattaa tarkistaa, jos käyttäjiä ei voi kirjautua sisään käyttäen monitasoisen todennuksen (MFA)

1. Ongelman kohdanneen käyttäjän on ehkä estetty Azure Active Directory Portal. Jos näin on, todennus yrittää kyseisen käyttäjän automaattisesti hylätään. [Noudata tämän artikkelin torjunnan purkamista.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Jos käyttäjän eston ollut apua tai ei ole estetty käyttäjä voi yrittää palauttaa käyttäjän MFA ja ne menevät läpi Rekisteröi uudelleen. [Noudattamalla tässä artikkelissa olevia ohjeita.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Jos tämä on ensimmäistä kertaa MFA käytössä ja käyttäjillä ei voi kirjautua sisään selaimet asiakkaita, kuten Outlook, Skype jne, ehkä ADAL (Active Directory Authentication kirjasto) ei ole käytössä tilauksesi O365. Tässä tapauksessa sinun on Exchange Online-Powershell muodostaa yhteyden ja suorittaa tämä cmdlet-komento:  *Set-OrganizationConfig-OAuth2ClientProfileEnabled: $true*