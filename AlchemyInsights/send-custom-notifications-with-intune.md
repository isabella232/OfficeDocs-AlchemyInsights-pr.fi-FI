---
title: Mukautettujen ilmoitusten lähettäminen Intunella
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720643"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="a17c0-102">Mukautettujen ilmoitusten lähettäminen hallittujen iOS-ja Android-laitteiden käyttäjille</span><span class="sxs-lookup"><span data-stu-id="a17c0-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="a17c0-103">Yritys portaali-sovellus käsittelee Intune-sovelluksen mukautetut ilmoitukset käyttäjän laitteessa.</span><span class="sxs-lookup"><span data-stu-id="a17c0-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="a17c0-104">Sovellus luo sitten push-ilmoituksen kyseiseen laitteeseen.</span><span class="sxs-lookup"><span data-stu-id="a17c0-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="a17c0-105">Seuraavat ovat laitteiden edellytykset, jotka tukevat mukautettujen ilmoitusten vastaanottamista, ja sovellus voi sitten luoda push-ilmoituksen:</span><span class="sxs-lookup"><span data-stu-id="a17c0-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="a17c0-106">Laitteessa on oltava asennettuna yritys portaali sovellus.</span><span class="sxs-lookup"><span data-stu-id="a17c0-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="a17c0-107">Laitteen on sallittava yritys portaali-sovelluksen lähettää push-ilmoituksia.</span><span class="sxs-lookup"><span data-stu-id="a17c0-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="a17c0-108">Kun sovellus on asennettu tai päivitetty, se pyytää käyttäjää sallimaan ilmoitukset.</span><span class="sxs-lookup"><span data-stu-id="a17c0-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="a17c0-109">Android-laitteissa on oltava asennettuna Google Play-Palvelut.</span><span class="sxs-lookup"><span data-stu-id="a17c0-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="a17c0-110">Laitteen on oltava rekisteröity Intunella.</span><span class="sxs-lookup"><span data-stu-id="a17c0-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="a17c0-111">Lisä tietoja viestin lähettämisestä on kohdassa [ominaisuuksien ohjeet](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="a17c0-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
