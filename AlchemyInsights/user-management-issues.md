---
title: Käyttäjien hallintaongelmat
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035532"
---
# <a name="user-management-issues"></a>Käyttäjien hallintaongelmat

**Mitä tapahtuu nykyisille määritetyille käyttäjille sovellukselle, jos poistan käyttäjämäärityksen pakollisen ominaisuuden käytöstä (asetan tämän ominaisuuden arvoksi Ei)?**

Käyttäjän **pakollisen tehtävän poistaminen käytöstä** EI vaikuta tällä hetkellä määritettyihin käyttäjiin. Jos poistat tämän ominaisuuden käytöstä, kaikki käyttäjät voivat käyttää sovellusta. Kaikki luettelossa mainitut käyttäjät ja ryhmille sovelluksessa määritetyt käyttäjät ovat edelleen kelvollisia.

- Jos haluat rajoittaa sovelluksen tietyille käyttäjille, katso kohta - Azure AD -sovelluksen rajoittaminen käyttäjäjoukolle [– Microsoftin käyttäjätietoympäristön | Microsoft Docs.](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.)
- Jos haluat määrittää käyttäjiä ja ryhmiä, azure Active Directoryn (Azure AD) yrityssovelluksiin joko Azure-portaalista tai PowerShellin avulla, katso lisätietoja artikkelista Sovelluksen käyttäjämäärityksen hallinta [Azure Active Directoryssa.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)
- Jos haluat delegoida sovellusten luonti- ja hallintaoikeuksia, katso kohta [Edustajasovelluksen hallinnan järjestelmänvalvojan oikeudet – Azure AD | Microsoft Docs.](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles)
- **Piilota tietyt yrityssovellukset käyttäjiltä** – Voit piilottaa kaikki Microsoft 365 -sovellukset **MyApps-paneelista** seuraavasti. Sovellukset näkyvät edelleen Office 365 -portaalissa.

 1. Kirjaudu Azure-portaaliin hakemiston yleisenä järjestelmänvalvojana. 
 2. Valitse **Azure Active Directory.** 
 3. Valitse **Käyttäjät**. 
 4. Valitse **Käyttäjäasetukset.** 
 5. Valitse **Yrityssovellukset-kohdassa** **Hallitse käyttäjien käynnistys- ja tarkastelemissovelluksia.** 
 6. Käyttäjät **näkevät Office 365 -sovellukset vain Office 365 -portaalissa, ja valitse** **Kyllä.** 
 7. Valitse **Tallenna**. 
 8. Lisätietoja on kohdassa [Yrityssovelluksen piilottaminen käyttäjäkokemukselta Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)

- Jos tarjoat Ohjelmisto palveluna (SaaS) -sovellusta useille organisaatioille, voit määrittää sovelluksesi hyväksymään minkä tahansa Azure Active Directory (Azure AD) -vuokraajan kirjautumiset. Tätä kokoonpanoa kutsutaan "sovelluksen moni vuokraajaksi". Minkä tahansa Azure AD -vuokraajan käyttäjät voivat kirjautua sovellukseesi, kun he ovat suostuneet käyttämään tiliään sovelluksessasi. Lisätietoja on kohdassa Azure [AD -käyttäjiin kirjautumisen sovellusten luominen – Microsoftin | Microsoft Docs.](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant)

- **Miten loppukäyttäjä voi käyttää sovellusta, kun hänet on määritetty sovellukseen?**

Jokaisella Enterprise-sovelluksen sovelluksella on linkki loppukäyttäjille. Käyttäjät voivat käyttää sovellusta myös **MyApps-portaalin** kautta helposti.

- **Haluatko tietää, mitä sovelluksia ja sovelluksia käyttäjät käyttävät?**

Voit ladata kirjautumisraportit viimeisten 30 päivän ajan **portal.azure.com > Azure Active Directorysta> Signins> lataa raportteja.**

- Lue, miten [voit myöntää vuokraajan laajuiselle järjestelmänvalvojalle](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) sovelluksen suostumuksen ja [määrittää, miten loppukäyttäjät hyväksyvät sovellukset.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)

- [Ymmärrät, miten suostumus toimii,](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) [ja hallitse sovellusten suostumusta.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests)


