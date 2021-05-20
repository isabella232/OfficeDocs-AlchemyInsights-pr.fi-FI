---
title: Microsoft Defender for Office 365
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
ms.openlocfilehash: 91d73853d3ea67d6c6954fffb32dd1428e3d9976
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545265"
---
# <a name="troubleshooting-microsoft-defender-for-office-365"></a><span data-ttu-id="be2cd-102">Microsoft Defender for Office 365</span><span class="sxs-lookup"><span data-stu-id="be2cd-102">Troubleshooting Microsoft Defender for Office 365</span></span>

- <span data-ttu-id="be2cd-103">**Huomaatko viipeitä viestin toimittamisessa?**</span><span class="sxs-lookup"><span data-stu-id="be2cd-103">**Do you notice delays in message delivery?**</span></span> <span data-ttu-id="be2cd-104">Käytä [Dynaaminen toimitus -vaihtoehtoa](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) Microsoft Defender for Office 365 turvalliset liitteet -käytännössä.</span><span class="sxs-lookup"><span data-stu-id="be2cd-104">Use the [Dynamic Delivery](/microsoft-365/security/office-365-security/dynamic-delivery-and-previewing) option in your Microsoft Defender for Office 365 Safe Attachments policy.</span></span> <span data-ttu-id="be2cd-105">Tämä auttaa välttämään viestien viiveitä ja suojaamaan vastaanottajia haitallisilta tiedostoilta.</span><span class="sxs-lookup"><span data-stu-id="be2cd-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="be2cd-106">**Haluatko ilmoittaa Microsoftille virheellisistä positiivisista tai epätosi-negatiivisista negatiivisista?**</span><span class="sxs-lookup"><span data-stu-id="be2cd-106">**Do you want to report false positives or false negatives to Microsoft?**</span></span> <span data-ttu-id="be2cd-107">Käytä [Submissions Exploreria.](https://protection.office.com/reportsubmission)</span><span class="sxs-lookup"><span data-stu-id="be2cd-107">Use [Submissions Explorer](https://protection.office.com/reportsubmission).</span></span>

<span data-ttu-id="be2cd-108">-\*\* Tiesitkö, että voit ottaa käyttöön turvallisten linkkien suojauksen organisaatiosi vastaanottajien välisissä sisäisissä sähköpostiviesteissä?\*\* Toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="be2cd-108">-\*\* Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?\*\* Follow these steps:</span></span>

  1. <span data-ttu-id="be2cd-109">Siirry yleisen [https://protection.office.com](https://protection.office.com) järjestelmänvalvojan tai suojauksen järjestelmänvalvojan tiliin ja kirjaudu sisään.</span><span class="sxs-lookup"><span data-stu-id="be2cd-109">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="be2cd-110">Valitse vasemman siirtymisruudun **Uhkien hallinta**-kohdassa **Käytännön** \> **turvalliset linkit**.</span><span class="sxs-lookup"><span data-stu-id="be2cd-110">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="be2cd-111">Valitse **käytäntö koko organisaatiota koskevat käytännöt** -osassa ja valitse **sitten Muokkaa**.</span><span class="sxs-lookup"><span data-stu-id="be2cd-111">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="be2cd-112">Ota **Asetukset**-kohdassa **Käytä turvallisia linkkejä organisaation sisällä lähetetyissä viesteissä -asetus.**</span><span class="sxs-lookup"><span data-stu-id="be2cd-112">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
