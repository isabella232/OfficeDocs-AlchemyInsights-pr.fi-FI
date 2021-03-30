---
title: Sovelluksen rekisteröintisovelluksen salaisia tai varmenteen ongelmia
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
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404457"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="416f6-102">Sovelluksen rekisteröintisovelluksen salaisia tai varmenteen ongelmia</span><span class="sxs-lookup"><span data-stu-id="416f6-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="416f6-103">Sovelluksen asiakassalaisuus vanhenee?</span><span class="sxs-lookup"><span data-stu-id="416f6-103">Application client secret expiring?</span></span>

<span data-ttu-id="416f6-104">Riippumatta siitä, miten rekisteröity sovellus luotiin, joko sovellusten rekisteröintiportaalin perusrekisteröintiprosessin kautta tai jos palvelun päänimi on luotu vuokraajassa sovelluksen suostumuksella, uusi asiakassalaisuus on luotava ennen nykyisen asiakkaan vanhenemista ja päivitettävä siihen liittyvässä sovelluskoodissa.</span><span class="sxs-lookup"><span data-stu-id="416f6-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="416f6-105">Enimmäiskelpoisuusaika on 2 vuotta.</span><span class="sxs-lookup"><span data-stu-id="416f6-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="416f6-106">Muistutuksena salainen arvo on tallennettava, koska se ei enää näy portaalin Sovelluksen rekisteröinti -sivulta poistumisen jälkeen.</span><span class="sxs-lookup"><span data-stu-id="416f6-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="416f6-107">Lisätietoja on pika-aloitustoimintossa: [Sovelluksen rekisteröiminen Microsoftin](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) käyttäjätietoympäristössä ja Parhaat käytännöt [Microsoftin käyttäjätietoympäristössä.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)</span><span class="sxs-lookup"><span data-stu-id="416f6-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="416f6-108">Lisätietoja on kohdassa [Azure AD -sovelluksen luominen & pääsivusto portaalissa – Microsoftin käyttäjätietoympäristö.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)</span><span class="sxs-lookup"><span data-stu-id="416f6-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
