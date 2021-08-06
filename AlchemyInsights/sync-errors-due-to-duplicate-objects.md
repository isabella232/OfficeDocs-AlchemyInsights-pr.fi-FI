---
title: 902 (Objektien kaksoiskappaleista johtuvat synkronointivirheet)
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
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998791"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Objektien kaksoiskappaleiden vuoksi johtuvat synkronointivirheet

Näyttöön voi tulla jokin seuraavista virhesanomista, kun hakemistosynkronointi Microsoft 365:

- Objektia ei voi päivittää Microsoft Online Services -palveluissa, koska seuraavilla tähän objektiin liitetyissä määritteissä on arvoja, jotka on jo liitetty toiseen paikalliseen hakemistoon.

- Microsoft Online Services -hakemistossa on jo synkronoitu objekti, jolla on sama välityspalvelimen osoite.

- Tätä objektia ei voi päivittää, koska seuraavien objektiin liittyvien määritteiden arvot voivat jo liittyä toiseen objektiin paikallisissa hakemistopalveluissa: UserPrincipalName.

Voit tunnistaa ja korjata ongelman lataamalla ja ajamalla [IdFix DirSync -virheenkorjaustyökalun.](https://github.com/Microsoft/idfix)

Lisätietoja on artikkelissa [KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)
