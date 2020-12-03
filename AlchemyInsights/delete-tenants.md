---
title: Vuokra ajan poistaminen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564484"
---
# <a name="delete-tenant"></a><span data-ttu-id="9b4cd-102">Vuokra ajan poistaminen</span><span class="sxs-lookup"><span data-stu-id="9b4cd-102">Delete tenant</span></span>

<span data-ttu-id="9b4cd-103">Jos haluat poistaa Azure-mainoksen, varmista seuraavat:</span><span class="sxs-lookup"><span data-stu-id="9b4cd-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="9b4cd-104">Olet hakemiston yleinen hallinnoija.</span><span class="sxs-lookup"><span data-stu-id="9b4cd-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="9b4cd-105">Et ole kirjautunut tilillä, joka sisältää oletus hakemiston, kuten contoso.onmicrosoft.com, kirjautuneen tilin, kuten admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="9b4cd-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="9b4cd-106">Poista kaikki kansiossa olevat aktiiviset sovellukset ennen niiden poistamista.</span><span class="sxs-lookup"><span data-stu-id="9b4cd-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="9b4cd-107">Jos haluat poistaa aktiivisia sovelluksia, siirry sovellusten rekisteröinteihin ja poista olemassa olevat sovellukset.</span><span class="sxs-lookup"><span data-stu-id="9b4cd-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="9b4cd-108">Minkään Microsoft Online-palvelun, kuten Microsoft Azuren, Office 365 tai Azuren AD Premiumin, käytössä ei ole aktiivisia paketteja.</span><span class="sxs-lookup"><span data-stu-id="9b4cd-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="9b4cd-109">Siirrä tilauksesi tai nopeuta aktiivisten pakettien peruutusta Azure-tuen ja laskutuksen kautta.</span><span class="sxs-lookup"><span data-stu-id="9b4cd-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="9b4cd-110">Lue lisää siitä, miten voit peruuttaa Office 365-ja Azure-tila uksia.</span><span class="sxs-lookup"><span data-stu-id="9b4cd-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="9b4cd-111">Lisä tietoja olemassa olevan tila uksen liittämisestä vuokraajaan on Ohje aiheessa Azure- [tila uksen liittäminen tai lisääminen Azure AD-vuokraajaan](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="9b4cd-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="9b4cd-112">Aktiivista käyttö oikeutta ei ole.</span><span class="sxs-lookup"><span data-stu-id="9b4cd-112">There are no Active license.</span></span> <span data-ttu-id="9b4cd-113">Lisä tietoja käyttö oikeuksien poistamisesta on Ohje aiheessa [tila uksen poistaminen käyttö oikeuden poistamiseksi](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="9b4cd-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="9b4cd-114">Hakemistossa ei ole muita aktiivisia käyttäjiä paitsi itseäsi yleisenä järjestelmänvalvojana, kun yrität poistaa Azure AD:n.</span><span class="sxs-lookup"><span data-stu-id="9b4cd-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="9b4cd-115">Poista kaikki muut aktiiviset käyttäjät, ja mukautetun toimi alue nimen riippuvuudet on myös poistettava, kuten admin@contoso.com-sovelluksessa luodut käyttäjät.</span><span class="sxs-lookup"><span data-stu-id="9b4cd-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="9b4cd-116">Lisä tietoja:</span><span class="sxs-lookup"><span data-stu-id="9b4cd-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="9b4cd-117">Poista Azure Active Directory tai tilaus, Katso lisä tietoja artikkelista [Azure Active Directoryn poistaminen](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="9b4cd-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="9b4cd-118">Sovellusten poistaminen hakemistosta on kohdassa [sovellusten poistaminen](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="9b4cd-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
