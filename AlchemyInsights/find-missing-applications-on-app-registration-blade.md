---
title: Puuttuvien sovellusten etsiminen Sovelluksen rekisteröinti -sovelluksesta
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 0dee7e44a8701e1df924b9657cce6cf9d90160e58277d667f6069a4cbcf87ce5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057099"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Puuttuvien sovellusten etsiminen Sovelluksen rekisteröinti -sovelluksesta

1. Sovelluksia ei löydä sovelluksen rekisteröintiportaalista.

    Jos sovellus on usean vuokraajan sovellus ja se on rekisteröity toiseen vuokraajaan, sitä ei näytetä Sovelluksen rekisteröinti -kohdassa. Voit kuitenkin löytää sen Enterprise Applications -lapa-kohdasta, kun sitä on käytetty (suostumuksen jälkeen) ja palvelun pääobjekti on luotu vuokraajaasi. Lisätietoja on kohdassa Sovellukset, [& palvelun pääobjektit Azure AD:ssä – Microsoftin käyttäjätietoympäristö.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. Sovellusten tarkasteleminen sovelluksen rekisteröintisovelluksessa ei onnistu, vaikka olet järjestelmänvalvoja.

    Varmista, että olet oikeassa hakemistossa Azure-portaalissa.
3. Sovellukseni ei näy Enterprise-sovellusten lapa -luettelossa, mutta se näkyy, kun kyselyssä käytetään PowerShell-komentoa.

    Joskus, kun poistat sovelluksen Azure-portaalista, se ei näy portaalissa, mutta sitä ei ole poistettu kokonaan. Lisätietoja on seuraavissa artikkeleissa:
    - Voit noutaa aiemmin poistettujen sovellusten luettelon ja nähdä, näkyykö sovellus luettelossa PowerShell-komennolla: **Get-AzureADDeletedApplication.** Lisätietoja on kohdassa [Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Jos haluat poistaa sovelluksen kokonaan, voit kokeilla seuraavaa PowerShellissä: **Remove-AzureADApplication -ObjectId.** Lisätietoja on kohdassa [Remove-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Vaihtoehtoisesti voit yrittää palauttaa poistetun sovelluksen käyttämällä seuraavaa PowerShell-komentoa: **Palauta AzureADDeletedApplication -ObjectId.** Lisätietoja on kohdassa [Restore-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. En löydä luetteloa kaikista valmiiksi asennetuista yrityssovelluksista uudessa Azure-vuokraajassani.

    Azure AD:ssä ei ole oletusarvoisesti esiasennettuja yrityssovelluksia. Sinun on lisättävä se manuaalisesti Uusi sovellus -vaihtoehdosta selaamalla sitä Azure AD :n valikoimasta tai lisäämällä muu kuin valikoimasovellus. Lisätietoja on kohdassa [Pika-aloitustoiminto: Sovelluksen lisääminen Azure Active Directory (Azure AD) -vuokraajaan.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Jos olet yleinen järjestelmänvalvoja, voit käyttää sovelluksiasi helposti Microsoft 365 [sovellusten käynnistintä](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher).
5. En löydä sovelluksia Omat sovellukset -portaalista.

    Varmista, että sovelluksia ei ole piilotettu Omat sovellukset -kokoelmasivulla. Lisätietoja on kohdassa [Kokoelmat (esikatselu) Omat sovellukset -portaalissa – Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)
6. Jos haluat käynnistää sovelluksia Omat sovellukset -portaalista, katso & sovellusten etsiminen Omat sovellukset [-portaalissa – Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)
7. Office 365 Mover-sovellus ei näy Enterprise Applications -sovelluksesta asennuksen jälkeen.

    Office 365 Mover -sovellus on multitenant-sovellus, jota ei tarvitse lisätä AAD:lle Enterprise App Registration -kohdan Valikoimasovellukset-osassa. Jos Office 365 Mover-sovellusta, kirjaudu sisään sovellukseen ja se pyytää käyttäjän suostumusta käyttöoikeuksien saaminen. Kun käyttäjä antaa suostumuksen, tämä sovellus lisätään automaattisesti vuokraajaan tunnuksella, jonka olet kirjautunut sisään.

    Kun olet kirjautunut sovellukseen, löydät tämän sovelluksen merkinnän Enterprise Applicationsin AAD-sovelluksesta. Sinun on haettava tätä sovellusta joko kirjoittamalla koko nimi eli "Office 365 Mover" tai yksinkertaisesti hakemalla hakusanalla "office" ja sen pitäisi luetella sovellus. Lisätietoja on kohdassa Office 365 Mover ilmoittaa, että se on jo asennettu, mutta sitä ei ole [lueteltu Enterprise-sovellusvalikoimassa.](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)
8. [Pika-aloitusopas: Tarkastele Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) -vuokraajaasi käyttäjätietojen hallintaa varten sovelluksista, jotka on jo määritetty käyttämään Azure AD -vuokraajaasi tunnistetietojen toimittajana (IdP).
9. [Sovelluksen lisäämiseen tai poistamiseen liittyviä yleisiä](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) ongelmia Azure Active Directory auttaa ymmärtämään yleisiä ongelmia, joita sovellusten tarkastelemiseen Azure Active Directory.
