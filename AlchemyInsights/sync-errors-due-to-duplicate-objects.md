---
title: 902 (Synkronointivirheet objektien kaksoiskappaleiden vuoksi)
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
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708059"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="84b51-102">Synkronointivirheet objektien kaksoiskappaleiden vuoksi</span><span class="sxs-lookup"><span data-stu-id="84b51-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="84b51-103">Näyttöön voi tulla jokin seuraavista virhesanomista, kun hakemistosynkronointi on valmis Microsoft 365:ssä:</span><span class="sxs-lookup"><span data-stu-id="84b51-103">You might receive one of the following error messages when directory synchronization finishes in Microsoft 365:</span></span>

- <span data-ttu-id="84b51-104">Tätä objektia ei voi päivittää Microsoft Online Services -palveluissa, koska seuraavilla tähän objektiin liitetyllä määritteellä on arvoja, jotka on jo liitetty toiseen paikalliseen hakemistoon.</span><span class="sxs-lookup"><span data-stu-id="84b51-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="84b51-105">Microsoft Online Services -palveluiden hakemistossa on jo synkronoitu objekti, jolla on sama välityspalvelimen osoite.</span><span class="sxs-lookup"><span data-stu-id="84b51-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="84b51-106">Tätä objektia ei voi päivittää, koska seuraavilla tähän objektiin liitetyllä määritteellä on arvoja, jotka voidaan jo liittää toiseen objektiin paikallisissa hakemistopalveluissa: UserPrincipalName.</span><span class="sxs-lookup"><span data-stu-id="84b51-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="84b51-107">Voit tunnistaa ja korjata ongelman lataamalla ja ajamalla [IdFix DirSync -virheenkorjaustyökalun.](https://github.com/Microsoft/idfix)</span><span class="sxs-lookup"><span data-stu-id="84b51-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://github.com/Microsoft/idfix).</span></span>

<span data-ttu-id="84b51-108">Lisätietoja on artikkelissa [KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)</span><span class="sxs-lookup"><span data-stu-id="84b51-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
