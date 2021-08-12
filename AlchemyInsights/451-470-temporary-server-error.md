---
title: 451 4.7.0 Tilapäinen palvelinvirhe. Yritä myöhemmin uudelleen. PRX4
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2021
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "3000003"
- "12465"
ms.openlocfilehash: ce898981d053c8b5dc080ee83434bdacd7f02a636f0183293915bacdb48ba4ef
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812578"
---
# <a name="451-470-temporary-server-error-please-try-again-later-prx4"></a>451 4.7.0 Tilapäinen palvelinvirhe. Yritä myöhemmin uudelleen. PRX4

Saatat kohdata ongelman, kun lähetät sähköpostia Smarthost smtp.office365.com -palvelun kautta SMTP-asiakaslähetyksen menetelmän avulla ja saat virhesanoman: "451 4.7.0 Väliaikainen palvelinvirhe. Yritä myöhemmin uudelleen. PRX4 on enimmäkseen tilapäinen." 

Varmista, että et käytä jaettua postilaatikkoa SMTP-asiakaslähetykseen, koska SMTP-asiakaslähetyksen menetelmä edellyttää lisensoituta postilaatikkoa sähköpostin lähettämiseen. Jos et kuitenkaan käytä jaettua postilaatikkoa ja ongelma jatkuu, tarkista seuraavat asiat:

1. Ota asiakkaan SMTP-lähetys käyttöön postilaatikossa, jota käytetään suorittamalla tämä PowerShell-komento:

    ```Set-CASMailbox -Identity sean@contoso.com -SmtpClientAuthenticationDisabled $false```

    TAI

    1. Siirry aktiiviset Microsoft 365 -hallintakeskus > **-valikkoon** ja valitse käyttäjä.
    1. Siirry Sähköposti-välilehteen > **sähköpostisovellukset >** **valitse Sähköpostisovellusten hallinta**. 
    1. Varmista, että **Todennettu SMTP** -asetus on valittuna (käytössä).
    1. Valitse **Tallenna muutokset**.
    
    Jos haluat ottaa SMTP-todennuksen käyttöön koko organisaatiossa, suorita tämä komento:

    `Set-TransportConfig -SmtpClientAuthenticationDisabled $true`
 
    **Huomautus:** tietoturvasyistä SMTP-todennus kannattaa ottaa käyttöön vain postilaatikossa. Käyttäjätason asetus korvaa organisaatiotason asetuksen.

2. Poista Azuren suojauksen oletusasetukset käytöstä valitsemalla Ota suojauksen oletusasetukset **käyttöön -asetus** **ei:**

    1. Kirjaudu Azure-portaaliin suojauksen järjestelmänvalvojana, ehdollisen käyttöoikeuden järjestelmänvalvojana tai yleisenä järjestelmänvalvojana.
    1. Siirry Azure Active Directory >**  -valikkoon** ja valitse **Suojauksen oletusasetusten hallinta**.
    1. Aseta Ota **käyttöön suojauksen oletusasetukset -asetuksen** arvoksi **Ei.**
    1. Valitse **Tallenna**.

3. Poista monimenetelmäinen todentaminen (MFA) käytöstä käytetyssä postilaatikossa.

    1. Siirry Microsoft 365 -hallintakeskus ja valitse vasemmassa siirtymisvalikossa **Käyttäjät,**  >  **jotka ovat aktiivisia.**
    1. Valitse **Aktiiviset käyttäjät** -sivulla **Monimenetelmäinen todentaminen**.
    1. Valitse käyttäjä ja poista **monimenetelmäinen todentaminen käytöstä.**

