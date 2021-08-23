---
title: Sovellukseni ei näy sovelluksen hallinnossa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454700"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Sovellukseni ei näy sovelluksen hallinnossa

Jos sovellus ei näy sovelluksenhallinnassa, tarkista seuraavat asiat:

1. Siirry [Azure AD:hen](https://aad.portal.azure.com/) ja etsi sovelluksen sovellustunnus etsimällä sovelluksen nimeä Yleiskatsaus-sivun yläpalkista.

1. Access Graph Resurssienhallinnassa ja hakea sovelluksen tunnusta palvelun pääobjektissa tämän kyselyn avulla ja korvaa vastaavalla sovellustunnuksella: <appId> < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. Jos tuloksia ei palauteta, hae sovellustunnusta sovelluksessa tämän kyselyn avulla ja korvaa asianmukainen <appId> sovellustunnus: < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

Jos kyselyssä ilmenee ongelmia, katso [tuki.](https://docs.microsoft.com/microsoft-365/business-video/get-help-support) 

Lisätietoja sovelluksista sovelluksen hallinnossa on kohdassa Lisätietoja näkyvyydestä ja [oivalluksista.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

Lisätietoja sovellusten tarkastelusta on kohdassa [Sovellusten tarkasteleminen.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps)
