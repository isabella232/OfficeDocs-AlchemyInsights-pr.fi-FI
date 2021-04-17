---
title: Education-asiakkaiden yleiset Teams-ongelmat
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
- "9000701"
- "3831"
- "3832"
ms.openlocfilehash: 6d1fac07673f6f945f382e4e640cf44afb76717d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51829445"
---
# <a name="teams-common-issues-for-education-customers"></a>Education-asiakkaiden yleiset Teams-ongelmat

**Education-asiakkaat**:

Jos tarvitset apua Teamsin käyttöönotossa etäopiskelun tukemiseen, siirry sivulle [FastTrack Center](https://www.microsoft.com/fasttrack) ja lähetä tukipyyntö. Tutustu seuraaviin Education-asiakkaiden yleisiin Teams-ongelmiin:

- Näetkö virheilmoituksen "**Älä jää paitsi!**"? varmista, että [Microsoft Teams on otettu käyttöön oppilaitoksessa](https://docs.microsoft.com/microsoft-365/education/intune-edu-trial/enable-microsoft-teams). Microsoft Teams ei ole oletusarvoisesti käytössä EDU-vuokraajissa, vaan se on otettava ensin käyttöön.

- **Oletko uusi Teams-käyttäjä?** Tutustu artikkeliin [Etäopetus ja -opiskelu Office 365 Educationissa](https://support.office.com/article/remote-teaching-and-learning-in-office-365-education-f651ccae-7b65-478b-8366-51bb884025c4) saadaksesi ajankohtaisimmat ohjeet oppilaitoksen määrittämiseen, tuntisuunnitteluun, virtuaalisiin tapaamisiin ja sisällön jakamiseen opiskelijoiden kanssa.

- Kun se on otettu käyttöön, käyttäjät voivat käyttää sitä joko asentamalla [työpöytäversion](https://docs.microsoft.com/MicrosoftTeams/get-clients#desktop-client) ja [mobiiliversion](https://docs.microsoft.com/MicrosoftTeams/get-clients#mobile-clients) tai selaimella osoitteessa https://teams.microsoft.com.

- **Teams-vieraskäytön salliminen**: tutustu [Teams-vieraskäytön tarkistuslistaan](https://docs.microsoft.com/microsoftteams/guest-access-checklist) ja varmista, että kaikki vaiheet on suoritettu.
    - [Tietoja vieraskäytöstä Microsoft Teamsissa](https://docs.microsoft.com/microsoftteams/guest-access)
    - [Asetukset – Microsoft Teams -vieraskäytön tarkistuslista](https://docs.microsoft.com/microsoftteams/guest-access-checklist)
    - [Vieraan liittyminen tiimiin](https://docs.microsoft.com/microsoftteams/guest-joins)

- **Teams-kokoukset ja liittyminen puhelimella**: Tarvitsetko apua puhelinneuvottelujen ottamisessa käyttöön tai määrittämisessä Microsoft Teamsissa? Onko tämä käyttäjä luotu hiljattain? Jos on, sinun tulee odottaa 2–24 tuntia, jotta asetukset tulevat voimaan. Jos haluat varmistaa, että käyttäjällä on puhelunneuvottelujen käyttöoikeus ja oletusarvoinen maksullinen numero:
    1. Siirry kohtaan Aktiiviset käyttäjät ja valitse haluamasi käyttäjä.
    2. Valitse hallintakeskuksen versiosta riippuen joko **Käyttöoikeudet ja sovellukset** tai valitse kohdassa **Tuotteiden käyttöoikeudet** **Muokkaa**.
    3. Varmista, että käyttäjällä on käyttöoikeus puhelinneuvotteluihin, Microsoft Teamsiin ja Skype for Business Onlineen (palvelupaketti 2).
    4. Valitse käyttäjän hallintakeskuksessa **Näytä kaikki** ja sitten **Teams**.
    5. Valitse Microsoft Teams -hallintakeskuksessa **Vanha portaali**.
    6. Valitse Skype for Business -hallintakeskuksessa **Puhelinneuvottelut** ja sitten **Käyttäjät**.
    7. Valitse haluamasi käyttäjä ja varmista, että käyttäjällä on oletusarvoinen maksullinen numero.

    Saat lisätietoja artikkelista [Microsoft Teams -puhelupalvelut](https://docs.microsoft.com/microsoftteams/calling-plans-for-office-365) tai soittamalla Microsoft Commerce Billing -tiimille, jos sinulla on käyttöoikeuksiin liittyviä kysymyksiä.

    Lisäresurssit

    - [Kokoukset ja konferenssit Microsoft Teamsissa](https://docs.microsoft.com/microsoftteams/deploy-meetings-microsoft-teams-landing-page)
    - [Puhelinneuvottelu](https://docs.microsoft.com/microsoftteams/audio-conferencing-in-office-365)

- **Kokouskäytännöt**: Kokouskäytäntöjen avulla hallitaan ominaisuuksia, jotka ovat kokouksen osallistujien käytössä organisaatiosi käyttäjien ajoittamissa kokouksissa. Kun olet luonut käytännön ja tehnyt haluamasi muutokset, voit määrittää käytäntöön käyttäjiä.

    - **Kokouskäytännön muuttaminen tai luominen**: Muuta kokouskäytäntöä tai luo käytäntö siirtymällä kohtaan **Microsoft Teams -hallintakeskus > Kokoukset > Kokouskäytännöt**. Valitse käytäntö luettelosta tai valitse **Lisää**. Jos luot uutta käytäntöä, kirjoita nimi ja kuvaus. Nimi ei voi sisältää erikoismerkkejä, ja sen pituus voi olla enintään 64 merkkiä. Valitse asetukset ja valitse sitten **Tallenna**. 
    
        Sinulla saattaa esimerkiksi olla joukko käyttäjiä, ja haluat rajoittaa kokouksen tarvitsemaa kaistanleveyttä. Tällöin voit luoda uuden käytännön nimeltä Rajoitettu kaistanleveys ja ottaa pois käytöstä seuraavat asetukset:

        Kohdassa **Ääni ja video**:
        - Poista käytöstä **Salli pilvitallennus**.
        - Poista käytöstä **Salli IP-video**.

        Kohdassa **Sisällön jakaminen**:

        - Poista näytön jakamistila käytöstä.
        - Poista käytöstä **Salli luonnoslehtiö**.
        - Poista käytöstä **Salli jaetut muistiinpanot**.

        Sen jälkeen **Määritä käytäntö käyttäjille**:

    1. Siirry Microsoft Teams -hallintakeskuksen vasemmanpuoleisessa siirtymisvalikossa kohtaan **Käyttäjät** ja valitse käyttäjä.
    2. Valitse käyttäjä napsauttamalla käyttäjänimen vasemmalta puolelta ja valitse sitten **Muokkaa asetuksia**.
    3. Valitse **Kokouskäytäntö**-kohdassa haluamasi käytäntö ja valitse sitten **Käytä**.

    Jos haluat määrittää käytännön samaan aikaan useille käyttäjille, saat lisätietoja artikkelista [Teams-käyttäjäasetusten joukkomuokkaaminen](https://docs.microsoft.com/microsoftteams/edit-user-settings-in-bulk).

    Voit myös toimia seuraavalla tavalla:
    1. Siirry Microsoft Teams -hallintakeskuksen vasemmanpuoleisessa siirtymisvalikossa kohtaan **Kokoukset > Kokouskäytännöt**.
    2. Valitse käytäntö napsauttamalla käytännön nimen vasemmalla puolella.
    3. Valitse **Hallitse käyttäjiä**.
    4. Etsi **Hallitse käyttäjiä** -ruudussa käyttäjää näyttönimellä tai käyttäjänimellä, valitse nimi ja valitse **Lisää**. Lisää muut haluamasi käyttäjät toistamalla tätä vaihetta.
    5. Kun olet lisännyt haluamasi käyttäjät, valitse **Tallenna**.

- **Puuttuvan valintapaneelin vianmääritys**:
    - Varmista, että käyttäjälle on määritetty [Teams-käyttöoikeus](https://docs.microsoft.com/MicrosoftTeams/assign-teams-licenses).
    - Varmista, että käyttäjälle on määritetty [puhelupalvelupaketti](https://docs.microsoft.com/MicrosoftTeams/calling-plan-landing-page).
    - Salli käyttäjille [Enterprise Voice](https://docs.microsoft.com/skypeforbusiness/skype-for-business-hybrid-solutions/plan-your-phone-system-cloud-pbx-solution/enable-users-for-enterprise-voice-online-and-phone-system-voicemail#to-enable-your-users-for-phone-system-in-office-365-voice-and-voicemail).

- **Teamsin sisäänkirjautumisongelmien vianmääritys**: Varmista ensin, että [Microsoft Teams -palvelu on kunnossa](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/servicehealth). Tarkista sitten yleiset virhekoodit ja lue artikkeli [Miksi minulla on vaikeuksia kirjautua Microsoft Teamsiin?](https://support.office.com/article/a02f683b-61a3-4008-9447-ee60c5593b0f) Sinun kannattaa ehkä myös tutustua artikkeliin [Käyttäjätietomallit ja todentaminen Microsoft Teamsissa](https://docs.microsoft.com/MicrosoftTeams/identify-models-authentication).
