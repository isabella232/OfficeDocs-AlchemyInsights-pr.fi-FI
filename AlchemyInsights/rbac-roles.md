---
title: 'RBAC-roolit '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923128"
---
# <a name="rbac-rules"></a>RBAC-säännöt

Jos näyttöön tulee käyttöoikeusvirhe: 

- Asiakkaalla, jolla on objektitunnus, ei ole oikeuksia suorittaa toimintoja **(koodi: Käyttöoikeusfailed):** kun yrität luoda resurssia, tarkista, että olet kirjautuneena sellaisen käyttäjän kanssa, jolla on määritetty rooli, jolla on resurssin kirjoitusoikeudet valitussa vaikutusalueessa. Jos esimerkiksi haluat hallita virtuaalikoneita resurssiryhmässä, [](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) sinulla pitäisi olla virtuaalikoneen avustajarooli resurssiryhmässä (tai päätason vaikutusalueessa). Luettelo kunkin valmiin roolin käyttöoikeuksista on kohdassa [Azure-resurssien sisäänrakennettuja rooleja.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)
- Sinulla ei ole oikeutta luoda tukipyyntöä: kun yrität luoda tai päivittää tukipyynnön, tarkista, että olet tällä hetkellä kirjautuneena sellaisen käyttäjän kanssa, jolla on Microsoft.Support/supportTickets/write-käyttöoikeus, kuten [tukipyynnön](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)osallistuja .
- Roolimäärityksiä ei voi enää luoda **(koodi: RoleAssignmentLimitExceeded):** kun yrität määrittää roolin, yritä vähentää roolien määrää määrittämällä rooleja ryhmille. Azure tukee enintään **2 000** roolitilausta.

Lisätietoja Azuren RBAC-rooleista on kohdassa [Azuren RBAC-roolit.](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support)
