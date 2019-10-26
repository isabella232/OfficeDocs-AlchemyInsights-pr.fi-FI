---
title: 1385-toimisto-365-hälytys-käytännöt
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: edff5a265cf31ce9a242f73ae7121ccb8b591d5f
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/25/2019
ms.locfileid: "36661293"
---
# <a name="office-365-alert-policies"></a><span data-ttu-id="abc32-102">Office 365-hälytys käytännöt</span><span class="sxs-lookup"><span data-stu-id="abc32-102">Office 365 Alert policies</span></span>

<span data-ttu-id="abc32-103">Office 365 Security & Compliance Centerissä on [oletusarvoiset hälytys käytännöt](https://docs.microsoft.com/office365/securitycompliance/alert-policies#default-alert-policies) , jotka laukaisevat ilmoituksia organisaatioille, joilla on Office 365 Enterprise tai Office 365 Yhdysvaltain hallituksen E1/G1, E3/G3 tai E5/G5-tilaus.</span><span class="sxs-lookup"><span data-stu-id="abc32-103">The Office 365 Security & Compliance Center offers [default alert policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies#default-alert-policies) that trigger alerts for organizations with an Office 365 Enterprise or Office 365 US Government E1/G1, E3/G3, or E5/G5 subscription.</span></span> <span data-ttu-id="abc32-104">Tämän vuoksi järjestelmänvalvojat voivat saada Office365Alerts@microsoft.com lähettämän ilmoitus Sähkö posti-ilmoituksen, jonka aihe on seuraavankaltainen: *hälytys käytännön nimi*.</span><span class="sxs-lookup"><span data-stu-id="abc32-104">Therefore, admins may receive an alert email notification sent by Office365Alerts@microsoft.com with a subject line such as "A low-severity alert: *name of alert policy*".</span></span> <span data-ttu-id="abc32-105">Hälytys ilmoituksia lähetetään, kun hälytyksiä käynnistetään tavallisiksi toiminnoille, kuten käyttäjille:</span><span class="sxs-lookup"><span data-stu-id="abc32-105">Alert notifications are sent when alerts are triggered for common activities, such as when users:</span></span>

- <span data-ttu-id="abc32-106">Luo Saapuneet-kansion säännöt, jotka välittää sähkö postia.</span><span class="sxs-lookup"><span data-stu-id="abc32-106">Create inbox rules that forward email.</span></span>
- <span data-ttu-id="abc32-107">Määritä käyttö oikeudet posti laatikkoonsa.</span><span class="sxs-lookup"><span data-stu-id="abc32-107">Assign permissions their mailbox.</span></span>
- <span data-ttu-id="abc32-108">Jakaa tai poistaa suuren määrän tiedostoja SharePoint-tiedostojen jakamisessa.</span><span class="sxs-lookup"><span data-stu-id="abc32-108">Share or delete a large number of files in SharePoint file sharing.</span></span>
- <span data-ttu-id="abc32-109">Luo eDiscovery-hakuja ja vie haku tuloksia.</span><span class="sxs-lookup"><span data-stu-id="abc32-109">Create eDiscovery searches and export search results.</span></span>

<span data-ttu-id="abc32-110">Voit tarkistaa ja toimia hälytyksellä:</span><span class="sxs-lookup"><span data-stu-id="abc32-110">To review and act on an alert:</span></span>

1. <span data-ttu-id="abc32-111">Siirry [suojaus & yhteensopivuus keskukseen](https://protection.office.com) ja Kirjaudu sisään.</span><span class="sxs-lookup"><span data-stu-id="abc32-111">Go to the [Security & Compliance center](https://protection.office.com) and sign in.</span></span>
2. <span data-ttu-id="abc32-112">Valitse **hälytykset** > **Näytä hälytykset**.</span><span class="sxs-lookup"><span data-stu-id="abc32-112">Click **Alerts** > **View alerts**.</span></span>
3. <span data-ttu-id="abc32-113">Napsauttamalla ilmoitusta saat näkyviin pikaikki-sivun, jossa on tietoja hälytystä.</span><span class="sxs-lookup"><span data-stu-id="abc32-113">Click an alert to display a flyout page with information about the alert.</span></span>

<span data-ttu-id="abc32-114">Voit tehdä hälytyksen, kuten [poistaa epäilyttävän Saapuneet-kansion säännön](https://docs.microsoft.com/office365/securitycompliance/responding-to-a-compromised-email-account).</span><span class="sxs-lookup"><span data-stu-id="abc32-114">You can take action on an alert, such as [removing a suspicious inbox rule](https://docs.microsoft.com/office365/securitycompliance/responding-to-a-compromised-email-account).</span></span> <span data-ttu-id="abc32-115">Voit myös yksinkertaisesti sulkea hälytyksen valitsemalla hälytyksen pikaikki-sivulta **Ratkaise** .</span><span class="sxs-lookup"><span data-stu-id="abc32-115">Or you can simply close the alert by clicking **Resolve** on the alert flyout page.</span></span>

<span data-ttu-id="abc32-116">Lisä tietoja hälytys käytäntöjen määrittämisestä ja Hallin nasta [on tässä artikkelissa](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span><span class="sxs-lookup"><span data-stu-id="abc32-116">For more information about configuring and managing alert policies, see  [this article](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span></span>

<span data-ttu-id="abc32-117">**Tärkeää**: ilmoitus Sähkö posti-ilmoituksia Microsoftilta ei koskaan pyydä sinua toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="abc32-117">**Important**: Alert email notifications from Microsoft will never ask you to do the following:</span></span>

- <span data-ttu-id="abc32-118">Anna sala sana</span><span class="sxs-lookup"><span data-stu-id="abc32-118">Provide a password</span></span>
- <span data-ttu-id="abc32-119">Tilin suojaus tietojen tarkistaminen</span><span class="sxs-lookup"><span data-stu-id="abc32-119">Verify the security details of your account</span></span>
- <span data-ttu-id="abc32-120">Todenna itsesi uudelleen</span><span class="sxs-lookup"><span data-stu-id="abc32-120">Re-authenticate yourself</span></span>

<span data-ttu-id="abc32-121">Jos saat Sähkö posti viestin näin, se ei lähetetty Microsoft ja olisi pidettävä phishing huijaus.</span><span class="sxs-lookup"><span data-stu-id="abc32-121">If you receive an email message like this, it was not sent by Microsoft and should be considered a phishing scam.</span></span> <span data-ttu-id="abc32-122">Jos näin tapahtuu, [Ilmoita siitä Microsoftille](https://docs.microsoft.com/office365/SecurityCompliance/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span><span class="sxs-lookup"><span data-stu-id="abc32-122">If that happens, please [report it to Microsoft](https://docs.microsoft.com/office365/SecurityCompliance/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span></span>