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
ms.openlocfilehash: 1209e59668bbe69fe88408933ae11b357b8d4f1a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687615"
---
# <a name="alert-policies"></a><span data-ttu-id="b9e57-102">Hälytyskäytännöt</span><span class="sxs-lookup"><span data-stu-id="b9e57-102">Alert policies</span></span>

<span data-ttu-id="b9e57-103">Microsoft 365:n tietoturva& Compliance Center issä on [oletushälytyskäytäntöjä,](https://docs.microsoft.com/office365/securitycompliance/alert-policies#default-alert-policies) jotka käynnistävät hälytykset organisaatioille, joilla on Office 365 Enterprise- tai Office 365 US Government E1/G1-, E3/G3- tai E5/G5-tilaus.</span><span class="sxs-lookup"><span data-stu-id="b9e57-103">The Microsoft 365 security & Compliance Center offers [default alert policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies#default-alert-policies) that trigger alerts for organizations with an Office 365 Enterprise or Office 365 US Government E1/G1, E3/G3, or E5/G5 subscription.</span></span> <span data-ttu-id="b9e57-104">Tämän vuoksi järjestelmänvalvojat voivat saada Office365Alerts@microsoft.com lähettämän ilmoitusilmoituksen, jonka aiherivi on "Matalan vakavuusilmoituksen: *hälytyskäytännön nimi".*</span><span class="sxs-lookup"><span data-stu-id="b9e57-104">Therefore, admins may receive an alert email notification sent by Office365Alerts@microsoft.com with a subject line such as "A low-severity alert: *name of alert policy*".</span></span> <span data-ttu-id="b9e57-105">Hälytysilmoitukset lähetetään, kun hälytyksiä käynnistetään yleisille toiminnoille, esimerkiksi silloin, kun käyttäjät:</span><span class="sxs-lookup"><span data-stu-id="b9e57-105">Alert notifications are sent when alerts are triggered for common activities, such as when users:</span></span>

- <span data-ttu-id="b9e57-106">Luo saapuneet-kansion sääntöjä, jotka välittävät sähköpostia.</span><span class="sxs-lookup"><span data-stu-id="b9e57-106">Create inbox rules that forward email.</span></span>
- <span data-ttu-id="b9e57-107">Määritä postilaatikon käyttöoikeudet.</span><span class="sxs-lookup"><span data-stu-id="b9e57-107">Assign permissions their mailbox.</span></span>
- <span data-ttu-id="b9e57-108">Jaa tai poista suuri määrä tiedostoja SharePoint-tiedostojen jakamisessa.</span><span class="sxs-lookup"><span data-stu-id="b9e57-108">Share or delete a large number of files in SharePoint file sharing.</span></span>
- <span data-ttu-id="b9e57-109">Luo eDiscovery-hakuja ja vie hakutulokset.</span><span class="sxs-lookup"><span data-stu-id="b9e57-109">Create eDiscovery searches and export search results.</span></span>

<span data-ttu-id="b9e57-110">Hälytyksen tarkistaminen ja sen mukaan toimiminen:</span><span class="sxs-lookup"><span data-stu-id="b9e57-110">To review and act on an alert:</span></span>

1. <span data-ttu-id="b9e57-111">Siirry [Suojaus-& yhteensopivuuskeskukseen](https://protection.office.com) ja kirjaudu sisään.</span><span class="sxs-lookup"><span data-stu-id="b9e57-111">Go to the [Security & Compliance center](https://protection.office.com) and sign in.</span></span>
2. <span data-ttu-id="b9e57-112">Valitse **Hälytykset** > **Näytä hälytykset**.</span><span class="sxs-lookup"><span data-stu-id="b9e57-112">Click **Alerts** > **View alerts**.</span></span>
3. <span data-ttu-id="b9e57-113">Napsauttamalla ilmoitusta saat näkyviin pikaikkunasivun, jossa on tietoja ilmoituksesta.</span><span class="sxs-lookup"><span data-stu-id="b9e57-113">Click an alert to display a flyout page with information about the alert.</span></span>

<span data-ttu-id="b9e57-114">Voit tehdä hälytyksen toimia, kuten [poistaa epäilyttävän Saapuneet-kansion säännön](https://docs.microsoft.com/office365/securitycompliance/responding-to-a-compromised-email-account).</span><span class="sxs-lookup"><span data-stu-id="b9e57-114">You can take action on an alert, such as [removing a suspicious inbox rule](https://docs.microsoft.com/office365/securitycompliance/responding-to-a-compromised-email-account).</span></span> <span data-ttu-id="b9e57-115">Voit myös sulkea ilmoituksen valitsemalla hälytyspikaikkunasivulla **Ratkaise.**</span><span class="sxs-lookup"><span data-stu-id="b9e57-115">Or you can simply close the alert by clicking **Resolve** on the alert flyout page.</span></span>

<span data-ttu-id="b9e57-116">Lisätietoja hälytyskäytäntöjen määrittämisestä ja hallinnasta on [tässä artikkelissa](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span><span class="sxs-lookup"><span data-stu-id="b9e57-116">For more information about configuring and managing alert policies, see  [this article](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span></span>

<span data-ttu-id="b9e57-117">**Tärkeää**: Microsoftin sähköposti-ilmoitukset eivät koskaan pyydä sinua tekemään seuraavaa:</span><span class="sxs-lookup"><span data-stu-id="b9e57-117">**Important**: Alert email notifications from Microsoft will never ask you to do the following:</span></span>

- <span data-ttu-id="b9e57-118">Salasanan anto</span><span class="sxs-lookup"><span data-stu-id="b9e57-118">Provide a password</span></span>
- <span data-ttu-id="b9e57-119">Tilin suojaustietojen vahvistaminen</span><span class="sxs-lookup"><span data-stu-id="b9e57-119">Verify the security details of your account</span></span>
- <span data-ttu-id="b9e57-120">Vahvista itsesi uudelleen</span><span class="sxs-lookup"><span data-stu-id="b9e57-120">Re-authenticate yourself</span></span>

<span data-ttu-id="b9e57-121">Jos saat sähköpostiviestin näin, Microsoft ei lähettänyt sitä, ja sitä tulisi pitää tietojenkalasteluhuijauksena.</span><span class="sxs-lookup"><span data-stu-id="b9e57-121">If you receive an email message like this, it was not sent by Microsoft and should be considered a phishing scam.</span></span> <span data-ttu-id="b9e57-122">Jos näin tapahtuu, [ilmoita siitä Microsoftille](https://docs.microsoft.com/office365/SecurityCompliance/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span><span class="sxs-lookup"><span data-stu-id="b9e57-122">If that happens, please [report it to Microsoft](https://docs.microsoft.com/office365/SecurityCompliance/report-junk-email-and-phishing-scams-in-outlook-on-the-web-eop).</span></span>