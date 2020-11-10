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
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982450"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="41ab4-102">Luettelon kohteiden kommentit</span><span class="sxs-lookup"><span data-stu-id="41ab4-102">Comments on List items</span></span>

<span data-ttu-id="41ab4-103">Käyttäjät voivat pian lisätä ja poistaa luettelon kohteiden kommentteja.</span><span class="sxs-lookup"><span data-stu-id="41ab4-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="41ab4-104">Käyttäjät voivat tarkastella kaikkia luettelon kohteen kommentteja ja suodattaa niiden näkymien välillä, jotka näyttävät kohteeseen liittyviä kommentteja tai toimintaa.</span><span class="sxs-lookup"><span data-stu-id="41ab4-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="41ab4-105">**Ajoitus** :</span><span class="sxs-lookup"><span data-stu-id="41ab4-105">**Timing** :</span></span>

<span data-ttu-id="41ab4-106">**Kohdennettu vapauttaminen** : asteittainen käyttöönotto loka kuun puoli välissä ja valmistuvan marraskuun puoli väliin mennessä.</span><span class="sxs-lookup"><span data-stu-id="41ab4-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="41ab4-107">**Vakio tiedote** : asteittainen lasku Kiito on marraskuun puoli välissä ja sen valmistumisesta joulu kuun alku puolella</span><span class="sxs-lookup"><span data-stu-id="41ab4-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="41ab4-108">**Käyttöönotto** : kohdennettu julkaiseminen koko organisaatiossa</span><span class="sxs-lookup"><span data-stu-id="41ab4-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="41ab4-109">Käyttäjien on huomioitava seuraavat asiat, ennen kuin he voivat lisätä ja poistaa kommentteja:</span><span class="sxs-lookup"><span data-stu-id="41ab4-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="41ab4-110">Kommentit noudattavat SharePointiin sisältyviä käyttö oikeus asetuksia.</span><span class="sxs-lookup"><span data-stu-id="41ab4-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="41ab4-111">Perinteiset luettelot, joita ei ole vielä suunniteltu nykyaikaisiin käyttö liittymään, kuten tehtävä luetteloihin, eivät saa tätä kommentointi ominaisuutta.</span><span class="sxs-lookup"><span data-stu-id="41ab4-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="41ab4-112">Teamsin luetteloiden kommentointi ei ole käytettävissä tässä julkaisussa.</span><span class="sxs-lookup"><span data-stu-id="41ab4-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="41ab4-113">Haku ei indeksoi kommentteja.</span><span class="sxs-lookup"><span data-stu-id="41ab4-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="41ab4-114">Järjestelmänvalvojat voivat poistaa tämän ominaisuuden käytöstä organisaatio tasolla, jos muutat **Commentsonlistitemsdisabled** -parametria, joka on käytössä **-spovuokraaja** PowerShell cmdlet-komentosovelmassa.</span><span class="sxs-lookup"><span data-stu-id="41ab4-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="41ab4-115">Tällä hetkellä ei ole mahdollista poistaa kommentointia käytöstä sivuston tai luettelon tasolla.</span><span class="sxs-lookup"><span data-stu-id="41ab4-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="41ab4-116">Toivomme, että nämä hallinta toiminnot ovat myöhemmässä päivityksessä todennäköisiä vuoden 2021 ensimmäisellä neljänneksellä.</span><span class="sxs-lookup"><span data-stu-id="41ab4-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
