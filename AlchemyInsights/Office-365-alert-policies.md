---
title: 1385-Office-365-Alert-käytännöt
ms.author: markjjo
author: markjjo
manager: lauraw
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1385"
- "3200002"
ms.assetid: ''
ms.openlocfilehash: 8821a2ee1ae2207de5d1604762badf43808373c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664023"
---
# <a name="alert-policies"></a><span data-ttu-id="9535f-102">Ilmoitus käytännöt</span><span class="sxs-lookup"><span data-stu-id="9535f-102">Alert policies</span></span>

<span data-ttu-id="9535f-103">Microsoft 365-tieto turva &-yhteensopivuus keskus tarjoaa [oletusarvoiset ilmoitus käytännöt](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) , jotka laukaisevat organisaatioiden ilmoitukset Office 365 Enterprise-tai Office 365 US Government E1/G1, E3/G3 tai E5/G5-tila uksesta.</span><span class="sxs-lookup"><span data-stu-id="9535f-103">The Microsoft 365 security & Compliance Center offers [default alert policies](https://docs.microsoft.com/microsoft-365/compliance/alert-policies#default-alert-policies) that trigger alerts for organizations with an Office 365 Enterprise or Office 365 US Government E1/G1, E3/G3, or E5/G5 subscription.</span></span> <span data-ttu-id="9535f-104">Tämän vuoksi järjestelmänvalvojat voivat saada Office365Alerts@microsoft.com lähettämän ilmoituksen Sähkö posti-ilmoituksen, jossa on aihe rivi, kuten "alhaisen tason Varoitus: *hälytys käytäntöjen nimi*".</span><span class="sxs-lookup"><span data-stu-id="9535f-104">Therefore, admins may receive an alert email notification sent by Office365Alerts@microsoft.com with a subject line such as "A low-severity alert: *name of alert policy*".</span></span> <span data-ttu-id="9535f-105">Ilmoitus ilmoitukset lähetetään, kun ilmoitukset käynnistyvät yleisistä toiminnoista, kuten silloin, kun käyttäjät:</span><span class="sxs-lookup"><span data-stu-id="9535f-105">Alert notifications are sent when alerts are triggered for common activities, such as when users:</span></span>

- <span data-ttu-id="9535f-106">Luo Saapuneet-kansion säännöt, jotka edelleenlähettää sähkö postia.</span><span class="sxs-lookup"><span data-stu-id="9535f-106">Create inbox rules that forward email.</span></span>
- <span data-ttu-id="9535f-107">Määritä käyttö oikeudet posti laatikolle.</span><span class="sxs-lookup"><span data-stu-id="9535f-107">Assign permissions their mailbox.</span></span>
- <span data-ttu-id="9535f-108">Jaa tai poista suuri määrä tiedostoja SharePointin tiedoston jakamisessa.</span><span class="sxs-lookup"><span data-stu-id="9535f-108">Share or delete a large number of files in SharePoint file sharing.</span></span>
- <span data-ttu-id="9535f-109">Luo eDiscoveryn hakuja ja vie haku tuloksia.</span><span class="sxs-lookup"><span data-stu-id="9535f-109">Create eDiscovery searches and export search results.</span></span>

<span data-ttu-id="9535f-110">Ilmoituksen tarkistaminen ja siihen liittyvät toimet:</span><span class="sxs-lookup"><span data-stu-id="9535f-110">To review and act on an alert:</span></span>

1. <span data-ttu-id="9535f-111">Siirry [tieto turva & yhteensopivuus keskukseen](https://protection.office.com) ja Kirjaudu sisään.</span><span class="sxs-lookup"><span data-stu-id="9535f-111">Go to the [Security & Compliance center](https://protection.office.com) and sign in.</span></span>
2. <span data-ttu-id="9535f-112">Valitse **ilmoitukset**  >  **Näytä ilmoitukset**.</span><span class="sxs-lookup"><span data-stu-id="9535f-112">Click **Alerts** > **View alerts**.</span></span>
3. <span data-ttu-id="9535f-113">Napsauta ilmoitusta, jos haluat näyttää avattavan sivun, jossa on tietoja ilmoituksesta.</span><span class="sxs-lookup"><span data-stu-id="9535f-113">Click an alert to display a flyout page with information about the alert.</span></span>

<span data-ttu-id="9535f-114">Voit tehdä ilmoituksen esimerkiksi [epäilyttävän Saapuneet-kansion säännön poistamisesta](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account).</span><span class="sxs-lookup"><span data-stu-id="9535f-114">You can take action on an alert, such as [removing a suspicious inbox rule](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account).</span></span> <span data-ttu-id="9535f-115">Voit myös sulkea ilmoituksen napsauttamalla **Ratkaise** -painiketta ilmoituksen avattavasta ilmoitus-sivulla.</span><span class="sxs-lookup"><span data-stu-id="9535f-115">Or you can simply close the alert by clicking **Resolve** on the alert flyout page.</span></span>

<span data-ttu-id="9535f-116">Lisä tietoja ilmoitus käytäntöjen määrittämisestä ja Hallin nasta on  [tässä artikkelissa](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).</span><span class="sxs-lookup"><span data-stu-id="9535f-116">For more information about configuring and managing alert policies, see  [this article](https://docs.microsoft.com/microsoft-365/compliance/alert-policies).</span></span>

<span data-ttu-id="9535f-117">**Tärkeää**: Microsoftin ilmoitusten Sähkö posti-ilmoitukset eivät koskaan pyydä sinua tekemään seuraavaa:</span><span class="sxs-lookup"><span data-stu-id="9535f-117">**Important**: Alert email notifications from Microsoft will never ask you to do the following:</span></span>

- <span data-ttu-id="9535f-118">Anna sala sana</span><span class="sxs-lookup"><span data-stu-id="9535f-118">Provide a password</span></span>
- <span data-ttu-id="9535f-119">Tilin tieto turva tietojen tarkistaminen</span><span class="sxs-lookup"><span data-stu-id="9535f-119">Verify the security details of your account</span></span>
- <span data-ttu-id="9535f-120">Todenna itsesi uudelleen</span><span class="sxs-lookup"><span data-stu-id="9535f-120">Re-authenticate yourself</span></span>

<span data-ttu-id="9535f-121">Jos saat Sähkö posti viestin tältä, Microsoft ei lähettänyt sitä, ja sitä tulisi pitää tietojenkalasteluhuijaukseksi.</span><span class="sxs-lookup"><span data-stu-id="9535f-121">If you receive an email message like this, it was not sent by Microsoft and should be considered a phishing scam.</span></span> <span data-ttu-id="9535f-122">Jos näin käy, [Ilmoita siitä Microsoftille](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span><span class="sxs-lookup"><span data-stu-id="9535f-122">If that happens, please [report it to Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span></span>