---
title: SMTP-todennusongelmien ratkaiseminen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 2d3f0f6b700c3e4485c9064fbaa4bcc165e92e17
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826412"
---
# <a name="solving-smtp-authentication-issues"></a><span data-ttu-id="756fd-102">SMTP-todennusongelmien ratkaiseminen</span><span class="sxs-lookup"><span data-stu-id="756fd-102">Solving SMTP authentication issues</span></span>

<span data-ttu-id="756fd-103">Jos saat virheilmoituksia 5.7.57 tai 5.7.3, kun yrität lähettää SMTP-sähköpostia ja todentaa sen asiakasohjelmalla tai sovelluksella, tarkista muutama asia:</span><span class="sxs-lookup"><span data-stu-id="756fd-103">If you are getting errors 5.7.57 or 5.7.3 when trying to send SMTP email and authenticate with a client or application, there are a few things you should check:</span></span>

- <span data-ttu-id="756fd-104">Todennettu SMTP-lähetys on ehkä poistettu käytöstä vuokraajassa tai postilaatikossa, jota yrität käyttää (tarkista molemmat asetukset).</span><span class="sxs-lookup"><span data-stu-id="756fd-104">Authenticated SMTP submission might be disabled in your tenant, or on the mailbox that you are trying to use (check both settings).</span></span> <span data-ttu-id="756fd-105">Lisätietoja on kohdassa Todennettua [SMTP-lähetystä koskevan todennuksen ottaminen käyttöön tai poistaminen käytöstä.](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission)</span><span class="sxs-lookup"><span data-stu-id="756fd-105">To read more, see [Enable or disable authenticated client SMTP submission](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission).</span></span>

- <span data-ttu-id="756fd-106">Tarkista, [onko Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) otettu käyttöön vuokraajassa; Jos se on käytössä, SMTP-todennus perustodennuksella (tunnetaan myös nimellä vanha; tämä käyttää käyttäjänimeä ja salasanaa) epäonnistuu.</span><span class="sxs-lookup"><span data-stu-id="756fd-106">Check whether [Azure Security Defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) are enabled for your tenant; if enabled, SMTP authentication using basic authentication (also known as legacy; this will use username and password) will fail.</span></span>
