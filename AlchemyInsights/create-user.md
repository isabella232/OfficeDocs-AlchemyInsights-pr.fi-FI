---
title: Käyttäjän luominen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 742ff857141d08031302fdcff7e49b3eef90e0f7
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50744972"
---
# <a name="create-user"></a>Käyttäjän luominen

**ILMOITUS:**

- [WebView-kirjautumistuen peruuttaminen Googlesta 4. tammikuuta 2021 alkaen.](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) Testaa, vaikuttaako sovellustesi yhteensopivuus [Googlen](https://go.microsoft.com/fwlink/?linkid=2157323) ohjeiden mukaisesti.
- Varmista, että käytät järjestelmän verkkonäkymää tai järjestelmäselainta, kun kirjaudut sisään käyttäjiisi kuluttaja-Google-tileillä. Lisätietoja on kohdassa Sovellukseen [kirjautumisongelmat vain Chrome-selaimella.](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)

**En voi luoda uutta käyttäjää Azure AD -hakemistossa**

1. Varmista, että sinulla on oikeus luoda uusi peruskäyttäjä. Vain yleinen järjestelmänvalvoja tai käyttäjän järjestelmänvalvojan rooli Azure Active Directoryssa (AD) voi luoda uuden peruskäyttäjän. Jos et ole jossakin näistä rooleista, pyydä järjestelmänvalvojaa lisäämään sinut näihin rooleihin tai luomaan uusi käyttäjätili.
1. Varmista, että käyttäjänimi on toimialueessa, joka on vahvistettu Azure AD:ssäsi. Jos Azure AD:ssä ei ole vahvistettuja mukautettuja toimialuenimiä, voit käyttää Azure AD:n alkuperäistä toimialuetta, joka päättyy *.onmicrosoft.com.
1. Varmista, että käyttäjänimi on toimialueella, jota ei ole liitetty Azure AD:han paikallisesta AD:stä. Käyttäjiä ei voi lisätä pilvipalveluun toimialuenimillä, jotka on liitetty paikallisesti.
1. Varmista, että toisella käyttäjällä tai yhteyshenkilöllä ei ole vielä käyttäjänimiä, jonka haluat määrittää uudelle käyttäjälle. Käyttäjien nimien on oltava yksilöllisiä Azure AD:ssä.
1. Tutustu [Azure AD:n rooleihin ja](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) järjestelmänvalvojiin Azure AD:ssä.
1. Katso Azure [AD:n](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) toimialuenimet.
1. Tarkista [valvontalokit,](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) jos haluat nähdä tarkempia tietoja äskettäin luodusta tai poistetuksi käyttäjästä, kuten toiminnon suorittavasta henkilöstä ja milloin.
1. Lisätietoja uusien käyttäjien lisäämisestä on ohjeaiheessa Uuden käyttäjän luominen [Azure-portaalissa Azure AD:ssä.](/azure/active-directory/active-directory-users-create-azure-portal)
1. [Azure AD:n järjestelmänvalvojan roolit:](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)Järjestelmänvalvojan roolin käyttöoikeudet Azure Active Directoryssa
1. Voit luoda [uuden käyttäjän myös Azure AD PowerShellin avulla.](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
