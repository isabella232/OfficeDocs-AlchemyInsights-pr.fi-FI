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
ms.openlocfilehash: 00b5821e2edad8b60ff60b1f85264d81c72277e4
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404416"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Puuttuvien sovellusten etsiminen Sovelluksen rekisteröinti -sovelluksesta

1. Sovellusten rekisteröintiportaalissa ei ole sovelluksia.

    Jos sovellus on usean vuokraajan sovellus ja se on rekisteröity toiseen vuokraajaan, se ei näy Sovelluksen rekisteröinti -kohdassa. Voit kuitenkin löytää sen Enterprise Applications -sovelluksesta, kun sitä on käytetty (suostumuksen jälkeen) ja palvelun päätoimi on luotu vuokraajassasi. Lisätietoja on kohdassa Sovellukset ja [& Azure AD :ssä – Microsoftin tunnistetietoympäristössä.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. Sovellusten tarkasteleminen sovelluksen rekisteröintisovelluksessa ei onnistu, vaikka olet järjestelmänvalvoja.

    Varmista, että olet oikeassa hakemistossa Azure-portaalissa.
3. Sovellukseni ei näy Yrityssovellusten lavat -kohdassa, mutta se näkyy, kun kyselen PowerShell-komentoa.

    Joskus kun poistat sovelluksen Azure-portaalista, se ei näy portaalissa, mutta sitä ei ole ehkä poistettu kokonaan. Lisätietoja on seuraavissa artikkeleissa:
    - Voit noutaa aiemmin poistettujen sovellusten luettelon ja nähdä, näkyykö sovellus luettelossa PowerShell-komennolla: **Get-AzureADDeletedApplication.** Lisätietoja on kohdassa [Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Jos haluat poistaa sovelluksen kokonaan, voit kokeilla seuraavaa PowerShellissä: **Remove-AzureADApplication -ObjectId.** Lisätietoja on kohdassa [Remove-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Vaihtoehtoisesti voit yrittää palauttaa poistetun sovelluksen käyttämällä seuraavaa PowerShell-komentoa: **Palauta AzureADDeletedApplication -ObjectId.** Lisätietoja on kohdassa [Restore-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. En löydä luetteloa kaikista valmiiksi asennetuista yrityssovelluksista uudessa Azure-vuokraajassani.

    Azure AD:ssä ei ole esiasennettuja yrityssovelluksia oletusarvoisesti. Sinun on lisättävä se manuaalisesti Uusi sovellus -vaihtoehdosta selaamalla sitä Azure AD -valikoimasta tai lisäämällä muu kuin valikoimasovellus. Lisätietoja on [pika-aloitustoiminnissa: Sovelluksen lisääminen Azure Active Directory (Azure AD) -vuokraajaan.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Jos olet yleinen järjestelmänvalvoja, voit käyttää sovelluksiasi helposti [Microsoft 365:n sovellusten käynnistyksessä.](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher)
5. En löydä sovelluksiaNi sovelluksia -portaalista.

    Varmista, että sovelluksia ei ole piilotettu Omat sovellukset -kokoelmasivulla. Lisätietoja on Omat sovellukset [-portaalin Kokoelmat (esikatselu) -kohdassa Azure AD:ssä.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)
6. Jos haluat käynnistää sovelluksia Omat sovellukset -portaalista, katso lisätietoja & sovellusten etsiminen Omat sovellukset [-portaalista – Azure AD.](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)
7. Office 365 Mover -sovellus ei näy Enterprise Applications -terissä asennuksen jälkeen.

    Office 365 Mover -sovellus on multitenant-sovellus, jota ei tarvitse lisätä AAD:lle Enterprise App Registration -kohdan Valikoimasovellukset-osiossa. Jos haluat käyttää Office 365 Mover -sovellusta, kirjaudu sovellukseen ja pyydä käyttäjän suostumusta käyttöoikeuksiin. Kun käyttäjä on antanut suostumuksen, tämä sovellus lisätään automaattisesti vuokraajaan tunnuksella, jonka olet kirjautunut sisään.

    Kun olet kirjautunut sovellukseen, sinun pitäisi löytää tämän sovelluksen merkintä Enterprise Applications -sovelluksen teristä AAD:ssä. Sinun on haettava sovellusta joko kirjoittamalla koko nimi, kuten "Office 365 Mover" tai yksinkertaisesti hakemalla "office" ja sen pitäisi luetella sovellus. Lisätietoja saat [Office 365 Moverin](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)mukaan se on jo asennettu, mutta sitä ei näy Enterprise-sovellusvalikoimassa.
8. [Pika-aloitus: Tarkastele azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) -vuokraajaasi käyttäen käyttäjätietojen hallintaa varten määritettyjen sovellusten luetteloa. Näet, miten voit tarkastella sovelluksia, jotka on jo määritetty käyttämään Azure AD -vuokraajaasi tunnistetietojen toimittajana (IdP).
9. [Sovelluksen Azure Active Directoryyn lisäämisen tai poistamisen](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) yleisimmät ongelmat auttavat ymmärtämään yleisiä ongelmia, joita sovellusten tarkasteleminen Azure Active Directoryssa aiheuttaa.
