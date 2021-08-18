---
title: Luo käyttäjä
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
ms.openlocfilehash: a144b172787563b1aa57bdec790df1805a13f078
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323283"
---
# <a name="create-user"></a>Luo käyttäjä

**ILMOITUS:**

- [WebView-kirjautumistuen peruuttaminen Googlesta 4. tammikuuta 2021 alkaen.](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) Testaa, vaikuttaako Googlen yhteensopivuuden testaamista koskevat ohjeet [sovelluksiin.](https://go.microsoft.com/fwlink/?linkid=2157323)
- Varmista, että käytät järjestelmän verkkonäkymää tai järjestelmäselainta, kun kirjaudut sisään käyttäjiisi kuluttaja-Google-tileillä. Lisätietoja on kohdassa [Sovellukseen kirjautumisongelmat vain Chrome-selaimella.](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)

**En voi luoda uutta käyttäjää Azure AD -hakemistoon**

1. Varmista, että sinulla on oikeus luoda uusi peruskäyttäjä. Vain yleinen järjestelmänvalvoja tai käyttäjän järjestelmänvalvojan Azure Active Directory (AD) voi luoda uuden peruskäyttäjän. Jos et kuulu näihin rooleihin, pyydä järjestelmänvalvojaa lisäämään sinut näihin rooleihin tai luomaan uusi käyttäjätili.
1. Varmista, että käyttäjänimi on Toimialueessa, joka on vahvistettu Azure AD:ssä. Jos Azure AD:ssä ei ole vahvistettuja mukautettuja toimialuenimiä, voit käyttää Azure AD:n alkuperäistä toimialuetta, jonka lopussa on *.onmicrosoft.com.
1. Varmista, että käyttäjänimi on toimialueella, jota ei ole liitetty Azure AD:iin paikallisesta AD:stä. Käyttäjiä ei voi lisätä pilvipalveluun toimialuenimillä, jotka on liitetty paikallisesti.
1. Varmista, että toisella käyttäjällä tai yhteyshenkilöllä ei ole vielä käyttäjänimiä, jonka haluat määrittää uudelle käyttäjälle. Käyttäjänimien on oltava yksilöllisiä Azure AD:ssä.
1. Tutustu [Azure AD:n rooleihin ja järjestelmänvalvojiin](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD:ssä.
1. Katso Azure [AD:n](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) toimialuenimet.
1. Tarkista [valvontalokit,](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) jos haluat nähdä tarkempia tietoja äskettäin luodusta tai poistetusta käyttäjästä, kuten toiminnon suorittavasta henkilöstä ja milloin.
1. Lisätietoja uusien käyttäjien lisäämisestä on kohdassa Uuden käyttäjän luominen Azure AD:ssä Azure-portaalin [avulla.](https://docs.microsoft.com/azure/active-directory/active-directory-users-create-azure-portal)
1. [Azure AD:n järjestelmänvalvojan roolit:](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)järjestelmänvalvojan roolin Azure Active Directory
1. Voit luoda uuden [käyttäjän myös Azure AD PowerShellin avulla.](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)
