---
title: Dynamics 365 Liiketoimintasäännöt - lomakkeelle ei polttavista liiketoimintasäännön lomakkeet
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/16/2019
ms.locfileid: "35747503"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>OnChange-tapahtuma ei toteudu, jos kentän arvo muutetaan ohjelmallisesti

*OnChange* -tapahtuma ei toteudu, jos kentän arvo muutetaan ohjelmallisesti käyttämällä *määrite.* [AsetaArvo](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) -menetelmä. Jos haluat sen jälkeen, kun olet määrittänyt arvon, sinun on käytettävä *OnChange* -tapahtuman tapahtumakäsittelijää *formContext.data.entity määrite.* [fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) -menetelmän koodissa.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
