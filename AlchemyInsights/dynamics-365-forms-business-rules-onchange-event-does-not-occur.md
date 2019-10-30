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
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/29/2019
ms.locfileid: "37769336"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="922e2-102">OnChange-tapahtumaa ei tapahdu, jos kenttää muutetaan ohjelmallisesti</span><span class="sxs-lookup"><span data-stu-id="922e2-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="922e2-103">*OnChange* -tapahtumaa ei tapahdu, jos kenttää muutetaan ohjelmallisesti käyttämällä *määritettä.* [SetValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) -menetelmällä.</span><span class="sxs-lookup"><span data-stu-id="922e2-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="922e2-104">Jos haluat, että *onChange* -tapahtuman tapahtumakäsittelijät suoritetaan sen jälkeen, kun olet määrittänyt arvon, sinun on käytettävä *formcontext. data. Entity-määritettä* [fireonchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) -menetelmä koodissa.</span><span class="sxs-lookup"><span data-stu-id="922e2-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
