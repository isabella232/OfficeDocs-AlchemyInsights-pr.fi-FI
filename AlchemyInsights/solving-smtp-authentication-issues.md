---
title: SMTP-todennuksen ja vianmäärityksen ottaminen käyttöön
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: f6f0228f6cdf7e07c9f439c54a7a2bd5364381c0e47dc80117bd964c5eafea61
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957205"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a>SMTP-todennuksen ja vianmäärityksen ottaminen käyttöön

Jos haluat ottaa SMTP-todennuksen käyttöön postilaatikossa tai saat "Asiakas ei todennettu"-, "Todennus epäonnistui" tai "SmtpClientAuthentication"-virheen, jossa on koodi 5.7.57 tai 5.7.3 tai 5.7.139, kun yrität välittää sähköpostia todentamalla laitteen tai sovelluksen Microsoft 365:llä, ratkaise ongelma näiden kolmen toiminnon avulla:

1. Poista [Azuren suojauksen oletusasetukset käytöstä](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) valitsemalla Ota suojauksen **oletusasetukset käyttöön -asetus** **ei.**

    a. Kirjaudu Azure-portaaliin suojauksen järjestelmänvalvojana, ehdollisen käyttöoikeuden järjestelmänvalvojana tai yleisenä järjestelmänvalvojana.<BR/>
    b. Siirry  **Azure Active Directory >-kansioon.**<BR/>
    c. Valitse **Suojauksen oletusasetusten hallinta**.<BR/>
    d. Määritä **Ota käyttöön suojauksen oletusasetukset -asetuksena** **Ei.**<BR/>
    e. Valitse **Tallenna**.

2. [Ota asiakkaan SMTP-lähetys](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) käyttöön lisensoilussa postilaatikossa.

    a. Siirry Microsoft 365 -hallintakeskus Aktiiviset **käyttäjät -valikkoon** ja valitse käyttäjä.<BR/>
    b. Siirry Sähköposti-välilehteen ja valitse **Sähköpostisovellukset-kohdassa** **Sähköpostisovellusten hallinta**.<BR/>
    d. Varmista, **että Todennettu SMTP** on valittuna (käytössä).<BR/>
    e. Valitse **Tallenna muutokset**.<BR/>

3. [Poista monimenetelmäinen todentaminen (MFA) käytöstä](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) lisensoilussa postilaatikossa.

    a. Siirry Microsoft 365 -hallintakeskus ja valitse vasemmassa siirtymisvalikossa **Käyttäjät,**  >  **jotka ovat aktiivisia.**<BR/>
    b. Valitse **Monimenetelmäinen todentaminen**.<BR/>
    c. Valitse käyttäjä ja poista **Multi-Factor auth käytöstä.**<BR/>
