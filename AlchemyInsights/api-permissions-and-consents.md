---
title: Ohjelmointirajapinnan käyttöoikeudet ja suostumus
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974604"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="eff7c-102">Ohjelmointirajapinnan käyttöoikeudet ja suostumus</span><span class="sxs-lookup"><span data-stu-id="eff7c-102">API permissions and consent</span></span>

<span data-ttu-id="eff7c-103">Microsoftin tunnistetietoympäristöön integroivat sovellukset noudattavat valtuutusmallia, jonka avulla käyttäjät ja järjestelmänvalvojat voivat hallita, miten tietoja voidaan käyttää.</span><span class="sxs-lookup"><span data-stu-id="eff7c-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="eff7c-104">Valtuutusmallin käyttöönotto on päivitetty Microsoftin tunnistetietoympäristön päätepisteeseen.</span><span class="sxs-lookup"><span data-stu-id="eff7c-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="eff7c-105">Se muuttaa tapaa, jolla sovelluksen on oltava vuorovaikutuksessa Microsoftin käyttäjätietoympäristön kanssa.</span><span class="sxs-lookup"><span data-stu-id="eff7c-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="eff7c-106">[Käyttöoikeudet ja suostumus Microsoftin](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) käyttäjätietoympäristön päätepisteissä kattavat tämän valtuutusmallin peruskäsitteet, mukaan lukien laajuus, käyttöoikeudet ja suostumus.</span><span class="sxs-lookup"><span data-stu-id="eff7c-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="eff7c-107">[Azure Active Directoryn (Azure AD) suostumuskehys](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) helpottaa usean vuokraajan verkko- ja alkuperäissovellusten kehittämistä.</span><span class="sxs-lookup"><span data-stu-id="eff7c-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="eff7c-108">Nämä sovellukset sallivat kirjautumisen azure AD -vuokraajan käyttäjätileillä, jotka ovat eri asia kuin se, johon sovellus on rekisteröity.</span><span class="sxs-lookup"><span data-stu-id="eff7c-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="eff7c-109">Heidän on ehkä myös päästä käyttämään verkkorajapintojen, kuten Microsoft Graphin ohjelmointirajapintaa (Azure AD:n, Intunen ja palveluiden käyttäminen Microsoft 365:ssä) ja muiden Microsoft-palveluiden ohjelmointirajapintojen lisäksi omia verkkorajapintojen lisäksi.</span><span class="sxs-lookup"><span data-stu-id="eff7c-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

