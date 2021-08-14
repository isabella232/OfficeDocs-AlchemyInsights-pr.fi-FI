---
title: Dynamics 365 Formsin liiketoimintasäännöt – Liiketoimintasääntö ei ole käytettävissä lomakkeessa
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947296"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>OnChange-tapahtumaa ei tapahdu, jos kenttää muutetaan ohjelmallisesti

*OnChange-tapahtumaa* ei tapahdu, jos kenttää muutetaan ohjelmallisesti määritteen *avulla.* [setValue-menetelmä.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) Jos haluat, että *OnChange-tapahtuman* tapahtumakäsittelijät suoritetaan sen jälkeen, kun olet määrittänyt arvon, sinun on käytettävä *koodissa formContext.data.entity-määritettä* [fireOnchange.](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange)

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
