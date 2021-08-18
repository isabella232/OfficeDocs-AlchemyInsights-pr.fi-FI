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
ms.openlocfilehash: 607e27c883f83b4b29347e764b8f2273cf0f117e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325384"
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

**Huomautus:** Kun järjestelmänvalvoja palauttaa käyttäjän salasanan Azure-portaalissa, jos käyttäjä on liitetty tai salasanojen hash synkronoitu, salasana kirjoitetaan takaisin paikalliseen. Tämä toiminto edellyttää Azure Premium -käyttöoikeutta (P1 tai P2), eikä sitä tällä hetkellä tueta Office-hallintaportaalissa.
