---
title: Estä sisäänkirjautuminen kaikille käyttäjille
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003536"
- "6445"
ms.openlocfilehash: b1596fdf463413a5b6714c48f4097e9552948070
ms.sourcegitcommit: d151b09064df3fb573ae07a387a08d98a9553b9b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807454"
---
# <a name="block-sign-in-for-all-users"></a><span data-ttu-id="3fc64-102">Estä sisäänkirjautuminen kaikille käyttäjille</span><span class="sxs-lookup"><span data-stu-id="3fc64-102">Block sign in for all users</span></span>

<span data-ttu-id="3fc64-103">Jos haluat estää kaikki käyttäjät kirjautumasta Officeen, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="3fc64-103">To block everyone from signing into Office, follow these steps:</span></span>

1. <span data-ttu-id="3fc64-104">Valitse hallinta keskuksessa käyttäjät, joilla on [ **Users**  >  **aktiivisia käyttäjiä**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="3fc64-104">In the admin center, go to [**Users** > **Active users**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
2. <span data-ttu-id="3fc64-105">Valitse kaikki käyttäjät valitsemalla **näyttö nimi** -kohdan vieressä oleva valinta merkki.</span><span class="sxs-lookup"><span data-stu-id="3fc64-105">Select all users by clicking the check mark next to **Display Name** .</span></span> <span data-ttu-id="3fc64-106">Varmista, että olet poista sen järjestelmänvalvojan tilin valinta, johon olet kirjautunut sisään.</span><span class="sxs-lookup"><span data-stu-id="3fc64-106">Ensure you uncheck the admin account you are logged in with.</span></span>
3. <span data-ttu-id="3fc64-107">Valitse **Vie käyttäjät** Muokkaa kirjautumistilaa-kohdan vieressä olevaa **"..."** -painiketta  >  **Edit sign-in status** ja valitse sitten **Estä käyttäjiä kirjautumasta** sisään.</span><span class="sxs-lookup"><span data-stu-id="3fc64-107">Click **"..."** next to **Export Users** > **Edit sign-in status** , then select **Block users from signing in** .</span></span> <span data-ttu-id="3fc64-108">Uudet kirjautumislaajennukset estetään heti.</span><span class="sxs-lookup"><span data-stu-id="3fc64-108">The new sign-ins are blocked immediately.</span></span> <span data-ttu-id="3fc64-109">Jos käyttäjä on jo kirjautunut sisään, käyttäjä kirjataan automaattisesti ulos kaikista Microsoftin palveluista 60 minuutin kuluessa.</span><span class="sxs-lookup"><span data-stu-id="3fc64-109">If a user was already signed in, then the user will be automatically signed out from all Microsoft services within 60 minutes.</span></span>
