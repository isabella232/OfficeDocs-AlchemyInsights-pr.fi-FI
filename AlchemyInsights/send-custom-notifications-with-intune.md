---
title: Mukautettujen ilmoitusten lähettäminen Intune-ominaisuuden avulla
ms.author: brenduns
author: brenduns
manager: dougeby
ms.date: 07/31/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000679
ms.openlocfilehash: 1244f07fd56cf603280f1710520a04d579224e44
ms.sourcegitcommit: 16f08d051afca3c6d0de32826324f91cf63ab5ba
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/16/2019
ms.locfileid: "36992310"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="0ce9d-102">Kuinka lähettää mukautettuja ilmoituksia hallittujen iOS-ja Android-laitteiden käyttäjille</span><span class="sxs-lookup"><span data-stu-id="0ce9d-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="0ce9d-103">Yritys portaali-sovellus käsittelee Intune-sovelluksen mukautetut ilmoitukset käyttäjän laitteessa.</span><span class="sxs-lookup"><span data-stu-id="0ce9d-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="0ce9d-104">Sovellus luo sitten push-ilmoituksen kyseiselle laitteelle.</span><span class="sxs-lookup"><span data-stu-id="0ce9d-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="0ce9d-105">Seuraavat ovat laitteen edellytyksiä, jotka tukevat mukautettujen ilmoitusten vastaanottoa, ja jotta sovellus luo push-ilmoituksen:</span><span class="sxs-lookup"><span data-stu-id="0ce9d-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="0ce9d-106">Laitteessa on oltava asennettuna yritys portaali-sovellus.</span><span class="sxs-lookup"><span data-stu-id="0ce9d-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="0ce9d-107">Laitteen on sallittava yritys portaali-sovelluksen lähettää push-ilmoituksia.</span><span class="sxs-lookup"><span data-stu-id="0ce9d-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="0ce9d-108">Kun sovellus on asennettu tai päivitetty, se kehottaa käyttäjää sallimaan ilmoitukset.</span><span class="sxs-lookup"><span data-stu-id="0ce9d-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="0ce9d-109">Android-laitteissa on oltava Google Play-Palvelut asennettuna.</span><span class="sxs-lookup"><span data-stu-id="0ce9d-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="0ce9d-110">Laite tulee rekisteröidä Intune.</span><span class="sxs-lookup"><span data-stu-id="0ce9d-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="0ce9d-111">Lisä tietoja, kuten viestin lähettäminen, on [ominaisuuden dokumentaatiossa](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="0ce9d-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
