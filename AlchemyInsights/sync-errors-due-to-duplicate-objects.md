---
title: 902 (Synkronoi objektien kaksoiskappaleiden aiheuttamat synkronointivirheet)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 6ea833e0c4aebe72bc5c02e3dc10c1edc4136dcc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767124"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Synkronoi objektien kaksoiskappaleiden aiheuttamat synkronointivirheet

Näyttöön saattaa tulla jokin seuraavista virhesanomista, kun hakemistosynkronointi on valmis Microsoft 365:ssä:

- Tätä objektia ei voi päivittää Microsoft Online Services -palveluissa, koska seuraavilla tähän objektiin liittyvillä määritteillä on arvoja, jotka on jo liitetty toiseen paikallisen hakemiston objektiin.

- Synkronoitu objekti, jolla on sama välityspalvelinosoite, on jo Microsoft Online Services -palveluiden hakemistossa.

- Objektia ei voi päivittää, koska seuraavilla tähän objektiin liittyvillä määritteillä on arvoja, jotka on jo liitetty toiseen paikalliseen hakemistopalveluiden objektiin: UserPrincipalName.

Voit tunnistaa ja korjata ongelman lataamalla ja suorittamalla [IdFix DirSync Error Remediation Tool -työkalun](https://www.microsoft.com/download/details.aspx?id=36832).

Lisätietoja on artikkelissa [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
