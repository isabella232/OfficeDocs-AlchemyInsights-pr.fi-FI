---
title: Ovatko käyttäjät saaneet haitallisia sähköpostiviestejä?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291789"
---
# <a name="did-your-users-receive-malicious-email"></a><span data-ttu-id="79583-102">Ovatko käyttäjät saaneet haitallisia sähköpostiviestejä?</span><span class="sxs-lookup"><span data-stu-id="79583-102">Did your users receive malicious email?</span></span>

- <span data-ttu-id="79583-103">Voit nyt raportoida haitalliset sähköpostiviestit Microsoftille käyttämällä [järjestelmänvalvojan viestejä tietoturva- ja yhteensopivuuskeskukselle](https://sip.protection.office.com/reportsubmission).</span><span class="sxs-lookup"><span data-stu-id="79583-103">You can now report the malicious email to Microsoft using the [Admin Submissions in Security & Compliance Center](https://sip.protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="79583-104">Tiedot, jotka lähetetään [järjestelmänvalvojan viesteinä](https://sip.protection.office.com/reportsubmission) tarkistetaan, ja tulokset näkyvät pikaikkunassa **lisätiedot**:</span><span class="sxs-lookup"><span data-stu-id="79583-104">Messages that are submitted in [admin submissions](https://sip.protection.office.com/reportsubmission) are scanned, and the following results shown in the **details** flyout:</span></span>

- <span data-ttu-id="79583-105">Jos lähettäjän sähköpostin todennus epäonnistui toimituksen aikana.</span><span class="sxs-lookup"><span data-stu-id="79583-105">If there was a failure in the sender's email authentication at the time of delivery.</span></span>
- <span data-ttu-id="79583-106">Tietoja kaikista käytäntöosumista, jotka ovat voineet vaikuttaa viestin päätökseen tai ohittaa sen.</span><span class="sxs-lookup"><span data-stu-id="79583-106">Information about any policy hits that could have affected or overridden the verdict of a message.</span></span>
- <span data-ttu-id="79583-107">Nykyiset tarkistustulokset, joista selviää, ovatko viestin URL-osoitteet tai tiedostot haitallisia.</span><span class="sxs-lookup"><span data-stu-id="79583-107">Current detonation results to see if the URLs or files contained in the message were malicious or not.</span></span>
- <span data-ttu-id="79583-108">Palaute arvostelijoilta</span><span class="sxs-lookup"><span data-stu-id="79583-108">Feedback from graders</span></span>

<span data-ttu-id="79583-109">Tarkistus suoritetaan uudelleen usean minuutin sisällä, jos ohitus löytyy.</span><span class="sxs-lookup"><span data-stu-id="79583-109">If an override was found, the rescan should complete in several minutes.</span></span> <span data-ttu-id="79583-110">Palautteessa voi kestää korkeintaan vuorokausi, jos sähköpostin todentamisessa ei ollut ongelmia tai ohitus ei vaikuttanut toimitukseen.</span><span class="sxs-lookup"><span data-stu-id="79583-110">If there wasn't a problem in email authentication or if the delivery wasn't affected by an override, then the feedback from graders could take up to a day.</span></span>

<span data-ttu-id="79583-111">Lähetä viesti uudelleen vuorokauden kuluttua tarkistusta varten, jos olet eri mieltä viestin, URL-osoitteen tai tiedoston (estetty tai ei estetty) lopullisesta päätöksestä.</span><span class="sxs-lookup"><span data-stu-id="79583-111">If you disagree with the final verdict on a message, URL or file (blocked vs. not blocked), submit the message again after a day for rescan.</span></span> <span data-ttu-id="79583-112">On mahdollista, että päätös muuttuu viestin uudelleen lähettämisen jälkeen.</span><span class="sxs-lookup"><span data-stu-id="79583-112">The chances are high that the verdict would change after submitting the message again.</span></span>

<span data-ttu-id="79583-113">Tällä välin voit poistaa haitallisia sähköpostiviestejä käyttäjien Saapuneet-kansioista noudattamalla [tämän artikkelin ohjeita](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span><span class="sxs-lookup"><span data-stu-id="79583-113">Meanwhile, you can remove malicious email from user inboxes by following the instructions in [this article](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).</span></span>

- <span data-ttu-id="79583-114">Office 365:n Microsoft Defenderin asiakkaat voivat:</span><span class="sxs-lookup"><span data-stu-id="79583-114">Customers with Microsoft Defender for Office 365 can:</span></span>
    - <span data-ttu-id="79583-115">käyttää [Threat Exploreria epäilyttävien sähköpostiviestien etsimiseen ja poistamiseen](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span><span class="sxs-lookup"><span data-stu-id="79583-115">use [Threat Explorer to Find and Delete Suspicious email](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)</span></span>
    - <span data-ttu-id="79583-116">[käyttää Turvallisia linkkejä estämään](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) haitallisten URL-osoitteiden käytön</span><span class="sxs-lookup"><span data-stu-id="79583-116">[use Safe Links to block access](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) to a malicious URL</span></span>
    - <span data-ttu-id="79583-117">jäljittää käyttäjät, jotka napsauttivat haitallisia URL-osoitteita:[Tietojenkalastelun URL-osoitteet ja napsautustiedot](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Hanki URL-seuranta](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span><span class="sxs-lookup"><span data-stu-id="79583-117">track users who clicked and accessed malicious URLs: [View phishing URL and click verdict data](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)</span></span>
    - <span data-ttu-id="79583-118">aloittaa manuaalisesti [automatisoitu tutkimus](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span><span class="sxs-lookup"><span data-stu-id="79583-118">manually [start an Automated Investigation](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)</span></span>

<span data-ttu-id="79583-119">Voit myös suojautua haitallisia URL-osoitteita ja tiedostoja vastaan noudattamalla näitä ohjeita:[Suojaus haitallisilta URL-osoitteilta ja tiedostoilta](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span><span class="sxs-lookup"><span data-stu-id="79583-119">You can also protect against malicious files and URLs by following the instructions in [Protection from malicious URLs and files](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).</span></span>