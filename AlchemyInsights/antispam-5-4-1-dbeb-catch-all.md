---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717358"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="08953-102">Virhe koodiin 550 5.4.1 Relay-käyttö estetty liittyvien ongelmien korjaaminen</span><span class="sxs-lookup"><span data-stu-id="08953-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="08953-103">Tämä ongelma ilmenee [, kun tarkistat, onko Sähkö posti osoite kelvollinen, jotta voit estää palautus viesteistä](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) , kun kirjoitat Microsoft Networkin.</span><span class="sxs-lookup"><span data-stu-id="08953-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="08953-104">Kokeile seuraavaa:</span><span class="sxs-lookup"><span data-stu-id="08953-104">Try the following:</span></span>

1. <span data-ttu-id="08953-105">Tarkista, koskeeko ongelma koko toimi aluetta vai yksittäistä Sähkö posti osoitetta:</span><span class="sxs-lookup"><span data-stu-id="08953-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="08953-106">Koko toimi alue: joskus toimi alue on synkronoitava. yritä [määrittää toimi alue sisäiseen käyttöön ja sitten takaisin arvovaltainen](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="08953-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="08953-107">Yksittäinen Sähkö posti osoite: joskus osoite on synkronoitava; SMTP-välitys palvelimen osoitteen vaihtamiseen ja sen vaihtamiseen takaisin voi olla apua.</span><span class="sxs-lookup"><span data-stu-id="08953-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="08953-108">Määrittää, koskeeko ongelma tiettyä ryhmää vai julkista kansiota.</span><span class="sxs-lookup"><span data-stu-id="08953-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="08953-109">Joidenkin objekti tyyppien objektit on ehkä luotava manuaalisesti Azure Active Directoryssa.</span><span class="sxs-lookup"><span data-stu-id="08953-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="08953-110">Jos tarvitset lisä ohjeita, voit avata tuki pyynnön ja määrittää ongelman laajuuden (mukaan lukien sen objektin tyypin, johon lähetät), jotta voimme auttaa sinua paremmin.</span><span class="sxs-lookup"><span data-stu-id="08953-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>