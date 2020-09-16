---
title: 902 (objektien kaksoiskappaleiden takia synkronointi virheet)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737338"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="92a8c-102">Objektien kaksoiskappaleita aiheuttavat synkronointi virheet</span><span class="sxs-lookup"><span data-stu-id="92a8c-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="92a8c-103">Näyttöön voi tulla jokin seuraavista virhe sanomista, kun hakemisto synkronointi on valmis Microsoft 365-sovelluksessa:</span><span class="sxs-lookup"><span data-stu-id="92a8c-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="92a8c-104">Objektia ei voi päivittää Microsoft Online Services-palveluissa, koska seuraavat tähän objektiin liittyvät määritteet sisältävät arvoja, jotka voivat olla jo liitettynä toiseen objektiin paikallisessa hakemistossa.</span><span class="sxs-lookup"><span data-stu-id="92a8c-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="92a8c-105">Microsoft Online Services-hakemistossa on jo synkronoitu objekti, jolla on sama välitys palvelin osoite.</span><span class="sxs-lookup"><span data-stu-id="92a8c-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="92a8c-106">Objektia ei voi päivittää, koska seuraavat tähän objektiin liittyvät määritteet sisältävät arvoja, jotka voivat olla jo liitettynä toiseen objektiin paikallisessa hakemisto palveluissa: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="92a8c-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="92a8c-107">Voit tunnistaa ja korjata ongelman lataamalla ja suorittamalla [IdFix DirSync-virheen korjaus työkalun](https://www.microsoft.com/download/details.aspx?id=36832).</span><span class="sxs-lookup"><span data-stu-id="92a8c-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="92a8c-108">Lisä tietoja on kohdassa [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span><span class="sxs-lookup"><span data-stu-id="92a8c-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
