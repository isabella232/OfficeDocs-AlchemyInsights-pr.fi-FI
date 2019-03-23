---
title: 902 (synkronointivirheet objektien kaksoisarvot vuoksi)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: eac74a6d4de58c9cdbdc8e8df8f705293bb12e87
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/22/2019
ms.locfileid: "30781259"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>Samanlaiset objektit synkronointivirheiden

Näyttöön tulee jokin seuraavista virhesanomista, kun directory-synkronointi on valmis:
  
- Ei voi päivittää tätä objektia Microsoft Online Services-palveluissa, koska tämän objektin liittyvät seuraavat määritteet ovat arvoja, jotka on ehkä jo liitetty toinen paikallinen hakemisto-objekti.
    
- Microsoft Online Services-kansiossa on jo synkronoitu objekti saman välityspalvelimen osoite.
    
- Objektia ei voi päivittää tätä, koska tämä objekti liittyy seuraavat määritteet ovat arvoja, jotka voi olla jo liitetty toiseen objektiin paikallisen-hakemistopalveluihin: UserPrincipalName.
    
Voit tunnistaa ja korjata ongelman, lataa ja suorita [IdFix DirSync virheen korjaus työkalu](https://www.microsoft.com/download/details.aspx?id=36832).
  
Lisätietoja on kohdassa [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).
  

