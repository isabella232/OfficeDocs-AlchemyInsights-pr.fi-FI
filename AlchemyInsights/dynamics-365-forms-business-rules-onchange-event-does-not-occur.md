---
title: 'Dynamics 365 Forms-liiketoiminta säännöt: lomakkeen liiketoiminta sääntö ei käynnisty'
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769336"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>OnChange-tapahtumaa ei tapahdu, jos kenttää muutetaan ohjelmallisesti

*OnChange* -tapahtumaa ei tapahdu, jos kenttää muutetaan ohjelmallisesti käyttämällä *määritettä.* [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) -menetelmällä. Jos haluat, että *onChange* -tapahtuman tapahtumakäsittelijät suoritetaan sen jälkeen, kun olet määrittänyt arvon, sinun on käytettävä *formcontext. data. Entity-määritettä* [fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) -menetelmä koodissa.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
