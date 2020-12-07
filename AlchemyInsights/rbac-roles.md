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
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583544"
---
# <a name="rbac-rules"></a>RBAC-säännöt

Jos saat käyttö oikeus virheen, toimi seuraavasti: 

- **Asiakkaalla, jolla on objekti tunnus, ei ole valtuutusta suorittaa toimenpiteitä vaikutus alueen kautta (koodi: Authorizatiepäonnistui)**: kun yrität luoda resurssin, tarkista, että olet kirjautuneena sellaisen käyttäjän kanssa, jolle on määritetty rooli, jolla on kirjoitus oikeudet valittuun käyttö alueen resurssiin. Jos haluat esimerkiksi hallita näennäiskoneita resurssi ryhmässä, sinulla pitäisi olla [näennäiskoneen avustaja](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) -rooli resurssi ryhmässä (tai pääkäyttö alue). Luettelo kunkin sisäisen roolin käyttö oikeuksista on kohdassa [Azure-resurssien sisäiset roolit](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- **Sinulla ei ole oikeutta luoda tuki pyyntöä**: kun yrität luoda tai päivittää tuki lippua, tarkista, että olet kirjautuneena käyttäjänä, jolle on määritetty rooli, jossa on Microsoft. support/supportTickets/Write-oikeus, kuten [tuki pyynnön avustaja](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- **Rooli määrityksiä ei voi luoda enempää (koodi: Roleassignmentlimitetceeded)**: kun yrität määrittää roolia, yritä vähentää rooli varausten määrää määrittämällä rooleja ryhmille. Azure tukee enintään **2000** -rooli määritystä pakettikohtaisesti.

Lisä tietoja Azure RBAC-rooleista on Ohje aiheessa [Azure RBAC-roolit](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
