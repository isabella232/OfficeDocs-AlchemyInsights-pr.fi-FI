---
title: Luettelon kohteiden kommentit
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
- "9003821"
- "6841"
ms.openlocfilehash: 2ee95e98aae3d9ec9a933f9cae234111d4285edd
ms.sourcegitcommit: 2eb1dd0856509b9907ccba9a5cb99d09b4f6eb4b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/21/2020
ms.locfileid: "49724151"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="3f509-102">Luettelon kohteiden kommentit</span><span class="sxs-lookup"><span data-stu-id="3f509-102">Comments on List items</span></span>

<span data-ttu-id="3f509-103">Käyttäjät voivat tarkastella kaikkia luettelon kohteen kommentteja ja suodattaa niiden näkymien välillä, jotka näyttävät kohteeseen liittyviä kommentteja tai toimintaa.</span><span class="sxs-lookup"><span data-stu-id="3f509-103">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="3f509-104">Käyttäjien on huomioitava seuraavat asiat, ennen kuin he voivat lisätä ja poistaa kommentteja:</span><span class="sxs-lookup"><span data-stu-id="3f509-104">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="3f509-105">Kommentit noudattavat SharePointiin sisältyviä käyttö oikeus asetuksia.</span><span class="sxs-lookup"><span data-stu-id="3f509-105">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="3f509-106">Perinteiset luettelot, joita ei ole vielä suunniteltu nykyaikaisiin käyttö liittymään, kuten tehtävä luetteloihin, eivät saa tätä kommentointi ominaisuutta.</span><span class="sxs-lookup"><span data-stu-id="3f509-106">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="3f509-107">Teamsin luetteloiden kommentointi ei ole käytettävissä tässä julkaisussa.</span><span class="sxs-lookup"><span data-stu-id="3f509-107">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="3f509-108">Haku ei indeksoi kommentteja.</span><span class="sxs-lookup"><span data-stu-id="3f509-108">Comments are not indexed by Search.</span></span>

<span data-ttu-id="3f509-109">Järjestelmänvalvojat voivat poistaa tämän ominaisuuden käytöstä organisaatio tasolla, jos muutat **Commentsonlistitemsdisabled** -parametria, joka on käytössä **-spovuokraaja** PowerShell cmdlet-komentosovelmassa.</span><span class="sxs-lookup"><span data-stu-id="3f509-109">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="3f509-110">Tällä hetkellä ei ole mahdollista poistaa kommentointia käytöstä sivuston tai luettelon tasolla.</span><span class="sxs-lookup"><span data-stu-id="3f509-110">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="3f509-111">Toivomme, että nämä hallinta toiminnot ovat myöhemmässä päivityksessä todennäköisiä vuoden 2021 ensimmäisellä neljänneksellä.</span><span class="sxs-lookup"><span data-stu-id="3f509-111">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
