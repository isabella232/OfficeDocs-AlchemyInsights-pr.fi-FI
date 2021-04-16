---
title: Ota käyttöön salasanan takaisinkirjoitus Azure AD Connectissa
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
- "9002933"
- "5615"
ms.openlocfilehash: 2ad7568bded3c8e4832e0e433a2d715e6307e4bb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814009"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a>Ota käyttöön salasanan takaisinkirjoitus Azure AD Connectissa

Jotta voit ottaa käyttöön salasanan palauttaminen takaisinkirjoituksen itsepalveluna, ota ensin käyttöön takaisinkirjoitusasetus Azure AD Connectissa. Suorita seuraavat vaiheet Azure AD Connect -palvelimelta:

1. Kirjaudu sisään Azure AD Connect -palvelimelle ja käynnistä **Azure AD Connectin** ohjattu määritys.
2. Klikkaa **Tervetuloa**-sivulla **Määritä**.
3. Valitse **Lisätehtävät**-sivulta **Mukauta synkronointivaihtoehtoja** ja klikkaa sitten **Seuraava**.
4. Lisää **Yhdistä Azure AD:hen** -sivulla yleisen Azure-vuokraajan järjestelmänvalvojan kirjautumistiedot ja klikkaa **Seuraava**.
5. Klikkaa **Yhdistä hakemistot**- ja **Toimialue/OU** -suodatussivuilta **Seuraava**.
6. Valitse **Valinnaiset ominaisuudet** -sivulla valintaruutu kohdasta **Salasanan takaisinkirjoitus** ja klikkaa **Seuraava**.
7. Klikkaa **Valmis määritettäväksi** -sivulta **Määritä** ja odota, että prosessi suoritetaan loppuun.
8. Kun määritys on suoritettu loppuun, klikkaa **Lopeta**.

Kun salasanan takaisinkirjoitus on otettu käyttöön Azure AD Connectissa, määritä Azure AD SSPR takaisinkirjoitusta varten.  Ota käyttöön salasanan takaisinkirjoitus SSPR:ssä suorittamalla seuraavat vaiheet:

1. Kirjaudu Azure-portaaliin yleisen järjestelmänvalvojan tilillä.
2. Etsi ja valitse **Azure Active Directory**, klikkaa **Salasanan palauttaminen** ja klikkaa sitten **Paikallinen integrointi**.
3. Valitse **Kirjoitetaanko salasanat takaisin paikalliseen hakemistoon?** -kohdasta **Kyllä**.
4. Valitse **Sallitaanko käyttäjien poistaa tilien lukituksen palauttamatta salasanojaan?** -kohdasta **Kyllä**.
5. Kun olet valmis, valitse **Tallenna**.

Lue lisää artikkelista [Azure Active Directoryn salasanan palauttamisen takaisinkirjoitus itsepalveluna paikalliseen ympäristöön](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).

> [!NOTE]
>  Kun järjestelmänvalvoja palauttaa käyttäjän salasanan Azure-portaalissa, jos käyttäjä on organisaation ulkopuolinen tai salasanan hajautus on synkronoitu, salasana kirjoitetaan takaisin paikallisesti. Tämä toiminto edellyttää Azure Premium -käyttöoikeutta (P1 tai P2), eikä sitä tällä hetkellä tueta Office-hallintaportaalissa.
