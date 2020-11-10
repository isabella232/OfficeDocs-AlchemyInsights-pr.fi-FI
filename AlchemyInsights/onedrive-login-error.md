---
title: OneDriven Kirjautumisvirhe AADSTS50011
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
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982449"
---
# <a name="onedrive-login-error-aadsts50011"></a><span data-ttu-id="52b32-102">OneDriven Kirjautumisvirhe AADSTS50011</span><span class="sxs-lookup"><span data-stu-id="52b32-102">OneDrive login error AADSTS50011</span></span>

<span data-ttu-id="52b32-103">Jos näyttöön tulee virhe ilmoitus "AADSTS50011: Pyynnössä määritetty vasta uksen URL-osoite ei vastaa vastausta" kun kirja udut sisään OneDrive-sovellukseen, tarkista seuraavat asiat:</span><span class="sxs-lookup"><span data-stu-id="52b32-103">If you receive an error "AADSTS50011: The reply URL specified in the request does not match the reply" when signing into the OneDrive app, check for the following:</span></span>

<span data-ttu-id="52b32-104">OneDrive-versiosi on oltava yhtä suuri tai suurempi kuin versio 20.052. XXXX. XXXX.</span><span class="sxs-lookup"><span data-stu-id="52b32-104">Your OneDrive version needs to be equal to or greater than version 20.052.XXXX.XXXX.</span></span> <span data-ttu-id="52b32-105">Jos haluat tarkistaa versiosi, napsauta ilmaisin alueella olevaa sinistä OneDrive-kuvaketta ja valitse **ohje & asetukset > asetukset > tietoja**.</span><span class="sxs-lookup"><span data-stu-id="52b32-105">To check your version, click on the blue OneDrive icon in the notification area, select **Help & Settings > Settings > About**.</span></span>

<span data-ttu-id="52b32-106">Verkostosi voi estää liikennettä **g.live.com** ja **oneclient.SFX.MS**.</span><span class="sxs-lookup"><span data-stu-id="52b32-106">Your network might block traffic to **g.live.com** and **oneclient.sfx.ms**.</span></span> <span data-ttu-id="52b32-107">Jos liikenne on estynyt, OneDrive ei voi päivittää itseään.</span><span class="sxs-lookup"><span data-stu-id="52b32-107">If that traffic is blocked, OneDrive cannot update itself.</span></span> <span data-ttu-id="52b32-108">Varmista verkonvalvojan kanssa, että sinulla on näiden URL-osoitteiden käyttäminen.</span><span class="sxs-lookup"><span data-stu-id="52b32-108">Work with your network administrator to ensure you have access to those URLs.</span></span> <span data-ttu-id="52b32-109">[Näiden pääte pisteiden](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) pitäisi olla tavoitettavissa asiakkaille, jotka käyttävät Microsoft 365-palvelu pakettia.</span><span class="sxs-lookup"><span data-stu-id="52b32-109">[These endpoints](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) should be reachable for customers using Microsoft 365 plans.</span></span>

<span data-ttu-id="52b32-110">Jos haluat hankkia OneDriven nykyisen version manuaalisesti, käy [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .</span><span class="sxs-lookup"><span data-stu-id="52b32-110">If you need to manually get a current version of OneDrive, visit [https://aka.ms/getonedrive](https://aka.ms/getonedrive).</span></span>
