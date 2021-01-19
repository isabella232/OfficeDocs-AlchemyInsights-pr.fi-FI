---
title: Järjestelmänvalvojan suostumusongelmat
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901128"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="8f3d5-102">Järjestelmänvalvojan suostumusongelmat</span><span class="sxs-lookup"><span data-stu-id="8f3d5-102">Admin consent issues</span></span>

1. <span data-ttu-id="8f3d5-103">Salli [järjestelmänvalvojan suostumustyönkulku,](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) jotta käyttäjät voivat pyytää järjestelmänvalvojan hyväksyntää suoraan suostumusnäytöstä.</span><span class="sxs-lookup"><span data-stu-id="8f3d5-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="8f3d5-104">Jos sinä tai sovelluksen käyttäjät näkevät odottamattomia virheitä hyväksyntäprosessin aikana, katso vianmääritysvaiheet tästä artikkelista: Odottamaton virhe sovelluksen [suostumuksen suorittamisessa.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)</span><span class="sxs-lookup"><span data-stu-id="8f3d5-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="8f3d5-105">Lue lisää [järjestelmänvalvojan suostumuksesta Microsoftin](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) käyttäjätietoympäristössä, miten suostumuskehote toimii ja miten koko vuokraajan järjestelmänvalvojan [suostumuspyyntöä voidaan arvioida.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="8f3d5-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="8f3d5-106">Microsoftin tunnistetietoympäristöön integroivat sovellukset noudattavat valtuutusmallia, jonka avulla käyttäjät ja järjestelmänvalvojat voivat hallita, miten tietoja voidaan käyttää.</span><span class="sxs-lookup"><span data-stu-id="8f3d5-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="8f3d5-107">Valtuutusmallin käyttöönotto on päivitetty Microsoftin käyttäjätietoympäristön päätepisteeseen, ja se muuttaa tapaa, jolla sovelluksen on oltava vuorovaikutuksessa Microsoftin käyttäjätietoympäristön kanssa.</span><span class="sxs-lookup"><span data-stu-id="8f3d5-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="8f3d5-108">Tutustu [käyttöoikeusmalliin,](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) mukaan lukien laajuus, käyttöoikeudet ja suostumus, tutustu Microsoftin käyttäjätietoympäristön päätepisteen käyttöoikeuksiin ja suostumukseen.</span><span class="sxs-lookup"><span data-stu-id="8f3d5-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>