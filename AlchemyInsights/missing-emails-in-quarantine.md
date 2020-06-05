---
title: Puuttuvat sähköpostit karanteenissa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569228"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="0a5e3-102">Puuttuvat sähköpostit karanteenissa"</span><span class="sxs-lookup"><span data-stu-id="0a5e3-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="0a5e3-103">Järjestelmänvalvojat voivat [tarkastella, vapauttaa tai poistaa näitä viestejä.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="0a5e3-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="0a5e3-104">Voit avata & Yhteensopivuuskeskuksen siirtymällä kohtaan [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="0a5e3-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="0a5e3-105">Voit avata Karanteeni-sivun suoraan siirtymällä kohtaan [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="0a5e3-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="0a5e3-106">Voit tehdä hakuja seuraavilla arvoilla:</span><span class="sxs-lookup"><span data-stu-id="0a5e3-106">You can search by the following values:</span></span>  

- <span data-ttu-id="0a5e3-107">**Sanoman tunnus**: Sanoman yleinen yksilöllinen tunnus.</span><span class="sxs-lookup"><span data-stu-id="0a5e3-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="0a5e3-108">Jos valitset viestin luettelosta, **Viestin tunnus -arvo** näkyy näkyviin tulevassa Tiedot-pikaikkunaruudussa. **Details**</span><span class="sxs-lookup"><span data-stu-id="0a5e3-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="0a5e3-109">Järjestelmänvalvojat voivat etsiä viestejä ja niitä vastaavia message id -arvoja [viestien jäljityksen](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) avulla.</span><span class="sxs-lookup"><span data-stu-id="0a5e3-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="0a5e3-110">**Lähettäjän sähköpostiosoite**: Yhden lähettäjän sähköpostiosoite.</span><span class="sxs-lookup"><span data-stu-id="0a5e3-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="0a5e3-111">**Vastaanottajan sähköpostiosoite**: Yksittäisen vastaanottajan sähköpostiosoite.</span><span class="sxs-lookup"><span data-stu-id="0a5e3-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="0a5e3-112">**Aihe**: Käytä viestin koko aihetta.</span><span class="sxs-lookup"><span data-stu-id="0a5e3-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="0a5e3-113">Hakuun ei ole merkitystä.</span><span class="sxs-lookup"><span data-stu-id="0a5e3-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="0a5e3-114">Kun olet syöttänyt hakuehdot, suodata tulokset valitsemalla ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Päivitä-painike Päivitä.**  </span><span class="sxs-lookup"><span data-stu-id="0a5e3-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="0a5e3-115">Karanteenissa olevien viestien ja tiedostojen tarkastelemiseen ja hallintaan käytettävät cmdlet-komennot ovat seuraavat:</span><span class="sxs-lookup"><span data-stu-id="0a5e3-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="0a5e3-116">Poista-Quarantine-läävä</span><span class="sxs-lookup"><span data-stu-id="0a5e3-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="0a5e3-117">Vienti-Karanteeni-lässä</span><span class="sxs-lookup"><span data-stu-id="0a5e3-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="0a5e3-118">Get-Quarantine-läävä</span><span class="sxs-lookup"><span data-stu-id="0a5e3-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="0a5e3-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Huomaa, että tämä cmdlet-komento on tarkoitettu vain viesteille, ei ATP:n haittaohjelmille SharePoint Onlinelle, OneDrive for Businessille tai Teamsille.</span><span class="sxs-lookup"><span data-stu-id="0a5e3-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="0a5e3-120">Julkaisu-Quarantine-lässä</span><span class="sxs-lookup"><span data-stu-id="0a5e3-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)