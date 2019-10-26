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
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/25/2019
ms.locfileid: "36529016"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="d084f-102">OnChange-tapahtumaa ei tapahdu, jos kenttää muutetaan ohjelmallisesti</span><span class="sxs-lookup"><span data-stu-id="d084f-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="d084f-103">*OnChange* -tapahtumaa ei tapahdu, jos kenttää muutetaan ohjelmallisesti käyttämällä *määritettä.* [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) -menetelmällä.</span><span class="sxs-lookup"><span data-stu-id="d084f-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="d084f-104">Jos haluat, että *onChange* -tapahtuman tapahtumakäsittelijät suoritetaan sen jälkeen, kun olet määrittänyt arvon, sinun on käytettävä *formcontext. data. Entity-määritettä.* [Fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) -metodin koodissa.</span><span class="sxs-lookup"><span data-stu-id="d084f-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
