---
title: 1385-Office-365-hälytyskäytännöt
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
ms.openlocfilehash: 05c58bded5ba45aef8ae3bc1d33491e6e0365c18
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502424"
---
# <a name="alert-policies"></a><span data-ttu-id="f41d2-102">Hälytyskäytännöt</span><span class="sxs-lookup"><span data-stu-id="f41d2-102">Alert policies</span></span>

<span data-ttu-id="f41d2-103">Microsoft 365 -tietoturva& Compliance Center sisältää [oletusvaroituskäytännöt,](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) jotka käynnistävät hälytykset organisaatioille, joilla on Office 365 Enterprise- tai Office 365 US Government E1/G1-, E3/G3- tai E5/G5-tilaus.</span><span class="sxs-lookup"><span data-stu-id="f41d2-103">The Microsoft 365 security & Compliance Center offers [default alert policies](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) that trigger alerts for organizations with an Office 365 Enterprise or Office 365 US Government E1/G1, E3/G3, or E5/G5 subscription.</span></span> <span data-ttu-id="f41d2-104">Siksi järjestelmänvalvojat voivat saada Office365Alerts@microsoft.com lähettämän ilmoitussähköposti-ilmoituksen, jossa on aiherivi, kuten "Vähävakavuusvaroitus: *hälytyskäytännön nimi".*</span><span class="sxs-lookup"><span data-stu-id="f41d2-104">Therefore, admins may receive an alert email notification sent by Office365Alerts@microsoft.com with a subject line such as "A low-severity alert: *name of alert policy*".</span></span> <span data-ttu-id="f41d2-105">Hälytysilmoitukset lähetetään, kun yleisiä toimintoja koskevat ilmoitukset käynnistyvät, esimerkiksi silloin, kun käyttäjät:</span><span class="sxs-lookup"><span data-stu-id="f41d2-105">Alert notifications are sent when alerts are triggered for common activities, such as when users:</span></span>

- <span data-ttu-id="f41d2-106">Luo saapuneet-kansion sääntöjä, jotka välittävät sähköpostia.</span><span class="sxs-lookup"><span data-stu-id="f41d2-106">Create inbox rules that forward email.</span></span>
- <span data-ttu-id="f41d2-107">Määritä postilaatikon käyttöoikeudet.</span><span class="sxs-lookup"><span data-stu-id="f41d2-107">Assign permissions their mailbox.</span></span>
- <span data-ttu-id="f41d2-108">Jaa tai poista suuri määrä tiedostoja SharePoint-tiedostojen jakamisessa.</span><span class="sxs-lookup"><span data-stu-id="f41d2-108">Share or delete a large number of files in SharePoint file sharing.</span></span>
- <span data-ttu-id="f41d2-109">Luo eDiscovery-haut ja vie hakutulokset.</span><span class="sxs-lookup"><span data-stu-id="f41d2-109">Create eDiscovery searches and export search results.</span></span>

<span data-ttu-id="f41d2-110">Voit tarkastella ja toimia hälytyksen perusteella:</span><span class="sxs-lookup"><span data-stu-id="f41d2-110">To review and act on an alert:</span></span>

1. <span data-ttu-id="f41d2-111">Siirry [Tietoturva-& Yhteensopivuus-keskukseen](https://protection.office.com) ja kirjaudu sisään.</span><span class="sxs-lookup"><span data-stu-id="f41d2-111">Go to the [Security & Compliance center](https://protection.office.com) and sign in.</span></span>
2. <span data-ttu-id="f41d2-112">Valitse **Hälytykset**  >  **Näytä hälytykset**.</span><span class="sxs-lookup"><span data-stu-id="f41d2-112">Click **Alerts** > **View alerts**.</span></span>
3. <span data-ttu-id="f41d2-113">Napsauttamalla ilmoitusta saat näkyviin pikaikkunasivun, jossa on tietoja ilmoituksesta.</span><span class="sxs-lookup"><span data-stu-id="f41d2-113">Click an alert to display a flyout page with information about the alert.</span></span>

<span data-ttu-id="f41d2-114">Voit tehdä hälytyksen, kuten [poistaa epäilyttävän Saapuneet-kansion säännön.](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)</span><span class="sxs-lookup"><span data-stu-id="f41d2-114">You can take action on an alert, such as [removing a suspicious inbox rule](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account).</span></span> <span data-ttu-id="f41d2-115">Voit myös sulkea ilmoituksen valitsemalla hälytyksen pikaikkunasivulla **Ratkaise.**</span><span class="sxs-lookup"><span data-stu-id="f41d2-115">Or you can simply close the alert by clicking **Resolve** on the alert flyout page.</span></span>

<span data-ttu-id="f41d2-116">Lisätietoja hälytyskäytäntöjen määrittämisestä ja hallinnasta on [tässä artikkelissa](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).</span><span class="sxs-lookup"><span data-stu-id="f41d2-116">For more information about configuring and managing alert policies, see  [this article](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).</span></span>

<span data-ttu-id="f41d2-117">**Tärkeää**: Microsoftin sähköposti-ilmoitusten ilmoittaminen ei koskaan pyydä sinua tekemään seuraavaa:</span><span class="sxs-lookup"><span data-stu-id="f41d2-117">**Important**: Alert email notifications from Microsoft will never ask you to do the following:</span></span>

- <span data-ttu-id="f41d2-118">Anna salasana</span><span class="sxs-lookup"><span data-stu-id="f41d2-118">Provide a password</span></span>
- <span data-ttu-id="f41d2-119">Tilin suojaustietojen vahvistaminen</span><span class="sxs-lookup"><span data-stu-id="f41d2-119">Verify the security details of your account</span></span>
- <span data-ttu-id="f41d2-120">Todenna itsesi uudelleen</span><span class="sxs-lookup"><span data-stu-id="f41d2-120">Re-authenticate yourself</span></span>

<span data-ttu-id="f41d2-121">Jos saat sähköpostiviestin näin, Microsoft ei lähettänyt sitä, ja sitä tulisi pitää tietojenkalasteluhuijauksena.</span><span class="sxs-lookup"><span data-stu-id="f41d2-121">If you receive an email message like this, it was not sent by Microsoft and should be considered a phishing scam.</span></span> <span data-ttu-id="f41d2-122">Jos näin käy, [ilmoita siitä Microsoftille](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span><span class="sxs-lookup"><span data-stu-id="f41d2-122">If that happens, please [report it to Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span></span>