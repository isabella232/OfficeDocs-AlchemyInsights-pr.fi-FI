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
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="020fb-102">OnChange-tapahtuma ei toteudu, jos kentän arvo muutetaan ohjelmallisesti</span><span class="sxs-lookup"><span data-stu-id="020fb-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="020fb-103">*OnChange* -tapahtuma ei toteudu, jos kentän arvo muutetaan ohjelmallisesti käyttämällä *määrite.* [AsetaArvo](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) -menetelmä.</span><span class="sxs-lookup"><span data-stu-id="020fb-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="020fb-104">Jos haluat sen jälkeen, kun olet määrittänyt arvon, sinun on käytettävä *OnChange* -tapahtuman tapahtumakäsittelijää *formContext.data.entity määrite.* [fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) -menetelmän koodissa.</span><span class="sxs-lookup"><span data-stu-id="020fb-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
