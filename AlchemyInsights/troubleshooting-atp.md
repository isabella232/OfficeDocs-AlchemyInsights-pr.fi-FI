---
title: Microsoft Defender for Office 365-vian määritys
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: 2c9543660056ebc02b0bd297f619f20fa6820093
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801440"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="9e520-102">Microsoft Defender for Office 365-vian määritys</span><span class="sxs-lookup"><span data-stu-id="9e520-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="9e520-103">Huomasitko viestin toimituksessa viiveitä?</span><span class="sxs-lookup"><span data-stu-id="9e520-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="9e520-104">Käytä ATP Safe-liitteiden käytössä olevaa [dynaamista toteutus](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) vaihtoehtoa.</span><span class="sxs-lookup"><span data-stu-id="9e520-104">Use the [Dynamic Delivery](https://docs.microsoft.com/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="9e520-105">Tämä auttaa välttämään viestin viiveitä ja suojaa samalla pahantahtoisten tiedostojen käyttäjiä.</span><span class="sxs-lookup"><span data-stu-id="9e520-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="9e520-106">Haluatko raportoida vääriä positiivisia tai vääriä negatiivisia tietoja Microsoftille?</span><span class="sxs-lookup"><span data-stu-id="9e520-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="9e520-107">Käytä tätä [linkkiä](https://www.microsoft.com/wdsi/filesubmission/) , kun haluat lähettää tiedostoja analyysia varten.</span><span class="sxs-lookup"><span data-stu-id="9e520-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="9e520-108">Tiesitkö, että voit ottaa käyttöön turvallisten linkkien suojauksen sisäiseen sähkö postiin, joka on lähetetty organisaation eri vastaanottajaidesi välillä?</span><span class="sxs-lookup"><span data-stu-id="9e520-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="9e520-109">Toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="9e520-109">Follow these steps:</span></span>

  1. <span data-ttu-id="9e520-110">Siirry [https://protection.office.com](https://protection.office.com) ja Kirjaudu sisään yleisen valvojan tai suojausvalvojan tilillä.</span><span class="sxs-lookup"><span data-stu-id="9e520-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="9e520-111">Valitse vasemman siirtymis ruudun **uhkien hallinta** -kohdassa **käytännön** \> **Turvalliset linkit** .</span><span class="sxs-lookup"><span data-stu-id="9e520-111">In the left navigation pane under **Threat management** , choose **Policy** \> **Safe Links** .</span></span>

  3. <span data-ttu-id="9e520-112">Valitse **koko organisaatio-osioon sovellettavat käytännöt** -kohdasta käytäntö ja valitse **Muokkaa** .</span><span class="sxs-lookup"><span data-stu-id="9e520-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit** .</span></span>

  4. <span data-ttu-id="9e520-113">Valitse **Asetukset** -kohdassa Ota käyttöön **Turvalliset linkit organisaatiossa lähetettyihin viesteihin** .</span><span class="sxs-lookup"><span data-stu-id="9e520-113">Under **Settings** , enable **Apply safe links to messages sent within the organization** .</span></span>
