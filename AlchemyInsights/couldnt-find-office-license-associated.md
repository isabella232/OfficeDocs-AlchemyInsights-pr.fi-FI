---
title: Office-sovellusten korjaaminen ei löytänyt Office-lisenssien liitettyä viestiä
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: 1820cdb83a1adf36b4e7d0898ecdf8097eb6f0f3
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627915"
---
# <a name="fixing-the-office-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="d1eac-102">Office-sovellusten korjaaminen ei löytänyt Office-lisenssejä liitetty-sanoma</span><span class="sxs-lookup"><span data-stu-id="d1eac-102">Fixing the Office apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="d1eac-103">Jos tämä sanoma tulee näyttöön, kokeile seuraavia:</span><span class="sxs-lookup"><span data-stu-id="d1eac-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="d1eac-104">Tarkista palo muuri-, virustentorjuntaohjelmisto-ja välitys palvelin asetukset ja varmista, etteivät ne estä Internet-pääsyä Office-sovelluksiin.</span><span class="sxs-lookup"><span data-stu-id="d1eac-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="d1eac-105">Katso [Office 365-URL-osoitteet ja IP-osoite alueet](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="d1eac-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="d1eac-106">Poista haavoittuvuuden sisältävän käyttäjän [Office-käyttö oikeus ja määritä se uudelleen](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) .</span><span class="sxs-lookup"><span data-stu-id="d1eac-106">Remove and [reassign the Office license](https://docs.microsoft.com/office365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="d1eac-107">Avaa Office-sovellus ja [Kirjaudu ulos](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) aiemmin luodusta käyttäjä tileistä.</span><span class="sxs-lookup"><span data-stu-id="d1eac-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="d1eac-108">Siirry Windows-asetuksiin > **tilit** > **Sähkö posti & tilit**ja poista kaikki työtilit paitsi haavoittuvuuden sisältävän tilin.</span><span class="sxs-lookup"><span data-stu-id="d1eac-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="d1eac-109">Siirry Windows-asetuksiin > **tilien** > **käyttö oikeus työ tai koulu**ja Katkaise kaikki työtilit lukuun ottamatta tiliä, jota haavoittuvuus koskee.</span><span class="sxs-lookup"><span data-stu-id="d1eac-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="d1eac-110">Palauta Officen aktivointi tila.</span><span class="sxs-lookup"><span data-stu-id="d1eac-110">Reset the Office activation state.</span></span> <span data-ttu-id="d1eac-111">[Ohjeet](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="d1eac-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="d1eac-112">[Kirjaudu sisään](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) haavoittuvuuden sisältävän käyttäjä tilin avulla.</span><span class="sxs-lookup"><span data-stu-id="d1eac-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="d1eac-113">Lisä vian määritys ratkaisuja on kohdassa [Officen käyttö oikeuden ja aktivointi virheiden poistaminen](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="d1eac-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>