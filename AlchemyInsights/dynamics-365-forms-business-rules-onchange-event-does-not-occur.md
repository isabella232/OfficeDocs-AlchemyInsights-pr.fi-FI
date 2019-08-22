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
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529016"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>OnChange-tapahtuma ei toteudu, jos kentän arvo muutetaan ohjelmallisesti

*OnChange* -tapahtuma ei toteudu, jos kentän arvo muutetaan ohjelmallisesti käyttämällä *määrite.* [AsetaArvo](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) -menetelmä. Jos haluat sen jälkeen, kun olet määrittänyt arvon, sinun on käytettävä *OnChange* -tapahtuman tapahtumakäsittelijää *formContext.data.entity määrite.* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) -menetelmän koodissa.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
