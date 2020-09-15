---
title: Puuttuvat sähkö postit karanteenissa
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
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673711"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="cf765-102">Puuttuvat sähkö postit karanteenissa "</span><span class="sxs-lookup"><span data-stu-id="cf765-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="cf765-103">Järjestelmänvalvojat voivat [tarkastella, vapauttaa tai poistaa näitä viestejä.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="cf765-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="cf765-104">Jos haluat avata tieto turva & yhteensopivuus keskuksen, siirry [https://protection.office.com](https://protection.office.com/) .</span><span class="sxs-lookup"><span data-stu-id="cf765-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="cf765-105">Jos haluat avata karanteeni sivun suoraan, siirry [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .</span><span class="sxs-lookup"><span data-stu-id="cf765-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="cf765-106">Voit hakea seuraavilla arvoilla:</span><span class="sxs-lookup"><span data-stu-id="cf765-106">You can search by the following values:</span></span>  

- <span data-ttu-id="cf765-107">**Viestin tunnus**: viestin yksilöivä tunnus.</span><span class="sxs-lookup"><span data-stu-id="cf765-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="cf765-108">Jos valitset viestin luettelosta,  **viestin tunnuksen**  arvo näkyy näkyviin tulevassa  **tiedot**  -pikaruudussa.</span><span class="sxs-lookup"><span data-stu-id="cf765-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="cf765-109">Järjestelmänvalvojat voivat etsiä viestejä ja niitä vastaavia viestin tunniste arvoja [viestin jäljityksen](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) avulla.</span><span class="sxs-lookup"><span data-stu-id="cf765-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="cf765-110">**Lähettäjän Sähkö posti osoite**: yksittäisen lähettäjän Sähkö posti osoite.</span><span class="sxs-lookup"><span data-stu-id="cf765-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="cf765-111">**Vastaanottajien Sähkö posti osoitteet**: yksi vastaanottajien Sähkö posti osoite.</span><span class="sxs-lookup"><span data-stu-id="cf765-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="cf765-112">**Aihe**: Käytä viestin koko aihetta.</span><span class="sxs-lookup"><span data-stu-id="cf765-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="cf765-113">Haussa kirjain koolla ei ole merkitsevä.</span><span class="sxs-lookup"><span data-stu-id="cf765-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="cf765-114">Kun olet lisännyt haku ehdot, ![ Suodata tulokset valitsemalla Päivitä-painike ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Päivitä** .  </span><span class="sxs-lookup"><span data-stu-id="cf765-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="cf765-115">Cmdlet-komennolla voit tarkastella ja hallita viestejä ja tiedostoja karanteenissa:</span><span class="sxs-lookup"><span data-stu-id="cf765-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="cf765-116">Poista-Karanteeninemessage</span><span class="sxs-lookup"><span data-stu-id="cf765-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="cf765-117">Vienti-Karanteeninemessage</span><span class="sxs-lookup"><span data-stu-id="cf765-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="cf765-118">Hanki-Karanteeninemessage</span><span class="sxs-lookup"><span data-stu-id="cf765-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="cf765-119">[Esikatselu-Quatarinemessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Huomaa, että tämä cmdlet on tarkoitettu vain viesteihin, ei Malware-tiedostoihin SharePoint Onlinen, OneDrive for Businessin tai teamsin kautta.</span><span class="sxs-lookup"><span data-stu-id="cf765-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="cf765-120">Tiedote-Karantiseinemessage</span><span class="sxs-lookup"><span data-stu-id="cf765-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)