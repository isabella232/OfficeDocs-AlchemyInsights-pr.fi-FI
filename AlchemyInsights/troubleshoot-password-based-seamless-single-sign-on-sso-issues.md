---
title: Salasanapohjaisen saumattoman kertakirjautumisen (SSO) ongelmien vianmääritys
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
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714766"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a><span data-ttu-id="e0b02-102">Salasanapohjaisen saumattoman kertakirjautumisen (SSO) ongelmien vianmääritys</span><span class="sxs-lookup"><span data-stu-id="e0b02-102">Troubleshoot Password-based Seamless Single Sign-on (SSO) issues</span></span>

<span data-ttu-id="e0b02-103">Lisätietoja salasanapohjaisen kirjautumisen perustoiminnot on ohjeaiheessa Salasanapohjainen todentaminen [Azure Active Directoryn avulla.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="e0b02-103">To learn the fundamentals of password-based SSO, see [Password-based authentication with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso).</span></span>

<span data-ttu-id="e0b02-104">**Salasanapohjaisen kirjautumisen määrittäminen**</span><span class="sxs-lookup"><span data-stu-id="e0b02-104">**Configure Password-based SSO**</span></span>

1. <span data-ttu-id="e0b02-105">[Salasanapohjaisen kertakirjautumisen määrittäminen](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) – Tässä artikkelissa on lisätietoja salasanapohjaisesta kertakirjautumisvaihtoehdosta.</span><span class="sxs-lookup"><span data-stu-id="e0b02-105">[Configure password-based single sign-on](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) - This article goes into more detail about the password-based SSO option.</span></span> <span data-ttu-id="e0b02-106">Jos lisäämässäsi sovelluksessa tarvitaan mukautettuja määrityksiä ja sinun on käytettävä salasanapohjaisia SSO-pohjaisia, tämä artikkeli on tarkoitettu sinulle.</span><span class="sxs-lookup"><span data-stu-id="e0b02-106">If the application you're adding requires custom configuration and you need to use password-based SSO, then this article is for you.</span></span>
2. <span data-ttu-id="e0b02-107">[Määritä salasanapohjainen kertakirjaus on-prem-sovelluksia](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) varten – Sovelluksen välityspalvelin tukee useita kertakirjaustiloja.</span><span class="sxs-lookup"><span data-stu-id="e0b02-107">[Configure password-based single sign on for on-prem apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) - Application Proxy supports several single sign-on modes.</span></span> <span data-ttu-id="e0b02-108">Salasanapohjainen kirjautuminen on tarkoitettu sovelluksille, jotka käyttävät todennusta käyttäjänimen ja salasanan yhdistelmää.</span><span class="sxs-lookup"><span data-stu-id="e0b02-108">Password-based sign-on is intended for applications that use a username/password combination for authentication.</span></span> <span data-ttu-id="e0b02-109">Kun määrität sovellukselle salasanapohjaisen kirjautumisen, käyttäjien on kirjauduttava paikalliseen sovellukseen kerran.</span><span class="sxs-lookup"><span data-stu-id="e0b02-109">When you configure password-based sign-on for your application, your users have to sign in to the on-premises application once.</span></span> <span data-ttu-id="e0b02-110">Tämän jälkeen Azure Active Directory tallentaa kirjautumistiedot ja antaa ne automaattisesti sovellukseen, kun käyttäjät voivat käyttää sitä etäyhteyden kautta.</span><span class="sxs-lookup"><span data-stu-id="e0b02-110">After that, Azure Active Directory stores the sign-in information and automatically provides it to the application when your users access it remotely.</span></span>
    - <span data-ttu-id="e0b02-111">Sovelluksen pitäisi olla jo julkaistu ja testattu sovelluksen välityspalvelimen avulla.</span><span class="sxs-lookup"><span data-stu-id="e0b02-111">You should already have published and tested your app with Application Proxy.</span></span> <span data-ttu-id="e0b02-112">Jos näin ei ole, noudata [Azure AD -sovelluksen](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) välityspalvelimen kautta julkaistavien sovellusten ohjeita ja jatka sitten salasanapohjaisen kirjautumisen määritystä esiasennettavalle sovellukselle.</span><span class="sxs-lookup"><span data-stu-id="e0b02-112">If not, follow the steps in [Publish applications using Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) then continue your configuration of password-based SSO for on-prem apps.</span></span>

<span data-ttu-id="e0b02-113">Lisätietoja salasanapohjaisen kertakirjautumisen vianmäärityksestä on ohjeaiheessa [Salasanapohjaisen kertakirjautumisen vianmääritys Azure AD:ssä](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span><span class="sxs-lookup"><span data-stu-id="e0b02-113">To troubleshoot password-based SSO, see [Troubleshoot password-based single sign-on in Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)</span></span>
