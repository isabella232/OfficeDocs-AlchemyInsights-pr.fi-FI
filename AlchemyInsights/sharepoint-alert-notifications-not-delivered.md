---
title: SharePoint-ilmoitusilmoituksia ei toimitettu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: a422805d11a128909e1be7bf5d08b24efc132e23
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742044"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="d4997-102">SharePoint-ilmoitusilmoituksia ei toimitettu</span><span class="sxs-lookup"><span data-stu-id="d4997-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="d4997-103">Tarkista roskapostin ROSKAPOSTI-kansio, sillä joskus hälytykset saattavat mennä sinne.</span><span class="sxs-lookup"><span data-stu-id="d4997-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="d4997-104">Määritä, **että kaikkia hälytyksiä ei toimiteta** tai jos tietyn tiedoston tai kirjaston **yksittäistä ilmoitusta** ei toimiteta.</span><span class="sxs-lookup"><span data-stu-id="d4997-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="d4997-105">**Yksittäisiä hälytyksiä ei toimiteta:** Jos tietyn tiedoston tai kirjaston yksittäistä ilmoitusta ei toimiteta, voit yrittää poistaa sen ja luoda sen uudelleen.</span><span class="sxs-lookup"><span data-stu-id="d4997-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="d4997-106">Lisätietoja ilmoituksen luomisesta on ohjeaiheessa [SharePoint-ilmoitusten hallinta, tarkasteleminen tai poistaminen.](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)</span><span class="sxs-lookup"><span data-stu-id="d4997-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="d4997-107">**Kaikkia hälytyksiä ei toimiteta:** Jos kaikkia useiden tiedostojen tai kirjastojen ilmoituksia ei toimiteta, tarkista SharePointin tai Exchangen yhteydessä mahdollisesti ilmenevistä tiedotteista/tapahtumista [palvelun kunnon hallintapaneelista.](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)</span><span class="sxs-lookup"><span data-stu-id="d4997-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="d4997-108">Ongelma voi johtua SharePoint-hälytysominaisuudesta tai viiveistä Exchangen kautta.</span><span class="sxs-lookup"><span data-stu-id="d4997-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="d4997-109">On myös tärkeää huomata, toimitetaanko muuta sähköpostia, ja jos ei, ongelma liittyy todennäköisesti Exchangen viivästyksiin.</span><span class="sxs-lookup"><span data-stu-id="d4997-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="d4997-110">Usein kysyttyjä kysymyksiä hälytyksistä:</span><span class="sxs-lookup"><span data-stu-id="d4997-110">FAQ on alerts:</span></span>

- <span data-ttu-id="d4997-111">Hälytyksiä ei voi lähettää jakeluryhmälle, vain suojaus- ja O365-ryhmiä tuetaan.</span><span class="sxs-lookup"><span data-stu-id="d4997-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="d4997-112">Hälytyssähköpostimalleja ei voi mukauttaa. sinun on käytettävä Microsoft FLOW- tai SharePoint Designer -työnkulkua niiden saavuttamiseksi.</span><span class="sxs-lookup"><span data-stu-id="d4997-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

<span data-ttu-id="d4997-113">Lisätietoja:</span><span class="sxs-lookup"><span data-stu-id="d4997-113">More Information:</span></span>

- <span data-ttu-id="d4997-114">**Hälytysten asetukset**: Lisätietoja ilmoitusten määrittämisestä on [ohjeaiheessa Ilmoituksen luominen, kun tiedosto tai kansio muuttuu SharePointissa](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span><span class="sxs-lookup"><span data-stu-id="d4997-114">**Alert setup**: For more information about setting up alerts, see [Create an alert to get notified when a file or folder changes in SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span></span>
- <span data-ttu-id="d4997-115">**Ilmoitusten vianmääritys**: Lisätietoja vianmääritysilmoituksista [on ohjeaiheessa Käyttäjät eivät saa SharePoint Online -ilmoitusilmoituksia](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).</span><span class="sxs-lookup"><span data-stu-id="d4997-115">**Troubleshoot alerts**: For more information about troubleshooting alerts, see [Users don't receive SharePoint Online alert notifications](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).</span></span>
- <span data-ttu-id="d4997-116">**O365:n vaatimustenmukaisuushälytyskäytännöt**ovat kohdassa Compliance Alert [Policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span><span class="sxs-lookup"><span data-stu-id="d4997-116">**Advanced O365 Compliance Alert Policies**: For more information about setting up these alerts, see [Compliance Alert Policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span></span>
- <span data-ttu-id="d4997-117">**SharePointin ja OneDriven valvontalokit**: Lisätietoja näiden tapahtumien noutamisesta [on ohjeaiheessa Valvontalokin etsiminen](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="d4997-117">**SharePoint and OneDrive Audit Logs**: For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
- <span data-ttu-id="d4997-118">**Advanced Threat Protectionin lähettämät hälytykset**: Katso [ATP SharePointia ja OneDrivea varten](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="d4997-118">**Alerts sent by Advanced Threat Protection**: See [ATP for SharePoint and OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
- <span data-ttu-id="d4997-119">**Tietojen menetyksen estämisen poliisien lähettämät ilmoitukset**: Katso [DLP-käytäntöjen sähköposti-ilmoitukset](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="d4997-119">**Alerts sent by Data Loss Prevention polices**: See [Email notifications for DLP policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

## <a name="related-topics"></a><span data-ttu-id="d4997-120">Aiheeseen liittyviä aiheita</span><span class="sxs-lookup"><span data-stu-id="d4997-120">Related Topics</span></span>

<span data-ttu-id="d4997-121">Haluatko kokeilla Microsoft Flow'ta SharePoint Onlinessa?</span><span class="sxs-lookup"><span data-stu-id="d4997-121">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="d4997-122">Luo työnkulku</span><span class="sxs-lookup"><span data-stu-id="d4997-122">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="d4997-123">SharePoint ja Flow</span><span class="sxs-lookup"><span data-stu-id="d4997-123">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
