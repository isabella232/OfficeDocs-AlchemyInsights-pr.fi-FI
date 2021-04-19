---
title: Teamsin kirjautumisvirhe AADSTS9000411
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821984"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="ec9aa-102">Teamsin kirjautumisvirhe AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="ec9aa-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="ec9aa-103">Kun kirjaudut Microsoft Teamsia, saatat saada virheilmoituksen: Valitettavasti AADSTS9000411 -kirjautumisessa on ongelmia: Pyyntöä ei ole muotoiltu **oikein. Parametri "login_hint" kopioidaan.**</span><span class="sxs-lookup"><span data-stu-id="ec9aa-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="ec9aa-104">Varmista ongelman ratkaisemiseksi, että Microsoft Teams -asiakasohjelmat on päivitetty.</span><span class="sxs-lookup"><span data-stu-id="ec9aa-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="ec9aa-105">Lisätietoja asiakkaan päivittämisestä on kohdassa [Microsoft Teamsin päivittäminen.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)</span><span class="sxs-lookup"><span data-stu-id="ec9aa-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="ec9aa-106">Jos asiakasohjelmaa ei jostain syystä voi päivittää, asiakkaan kirjaaminen ulos tyhjentää useimmat välimuistiin tallennetut tiedot.</span><span class="sxs-lookup"><span data-stu-id="ec9aa-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="ec9aa-107">Jos kirjautumisen jälkeen on kuitenkin edelleen ongelmia, sulje Teams ja tyhjennä asiakasvälimuisti seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="ec9aa-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="ec9aa-108">Sulje Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ec9aa-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="ec9aa-109">Siirry kansioon %appdata%\microsoft\teams ja poista kaikki tiedostot.</span><span class="sxs-lookup"><span data-stu-id="ec9aa-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="ec9aa-110">Avaa Microsoft Teams uudelleen.</span><span class="sxs-lookup"><span data-stu-id="ec9aa-110">Reopen Microsoft Teams.</span></span>
