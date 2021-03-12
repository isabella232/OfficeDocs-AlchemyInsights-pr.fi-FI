---
title: Esimerkki Microsoft Defender for Office 365:n turvallisten liitteiden käytännön käytöstä
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745997"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="87862-102">Esimerkki Microsoft Defender for Office 365:n turvallisten liitteiden käytännön käytöstä</span><span class="sxs-lookup"><span data-stu-id="87862-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="87862-103">Näillä asetuksilla otetaan käyttöön *Ei viiveitä* -niminen käytäntö, joka toimittaa viestit heti ja ottaa sitten liitteet uudelleen käyttöön skannatun tiedoston jälkeen:</span><span class="sxs-lookup"><span data-stu-id="87862-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="87862-104">**Nimi**: Ei viiveitä</span><span class="sxs-lookup"><span data-stu-id="87862-104">**Name**: No delays</span></span>
- <span data-ttu-id="87862-105">**Kuvaus:** Toimittaa viestit heti ja ottaa liitteet uudelleen käyttöön tarkistuksen jälkeen.</span><span class="sxs-lookup"><span data-stu-id="87862-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="87862-106">**Vastaus:** Valitse **Dynaaminen toimitus -vaihtoehto.**</span><span class="sxs-lookup"><span data-stu-id="87862-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="87862-107">Lisätietoja on kohdassa Dynaaminen [toimitus turvallisten liitteiden käytännöistä.](https://go.microsoft.com/fwlink/?linkid=2092328)</span><span class="sxs-lookup"><span data-stu-id="87862-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="87862-108"> Uudelleenohjausliite-osa: Valitse Ota uudelleenohjaus käyttöön ja kirjoita sitten microsoft 365:n yleisen järjestelmänvalvojan, suojauksen järjestelmänvalvojan tai suojausanalyytikon sähköpostiosoite, joka tutkii vahingollisia liitteitä.</span><span class="sxs-lookup"><span data-stu-id="87862-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="87862-109">**Applied To** section: **Select The recipient domain is,** and then select your domain.</span><span class="sxs-lookup"><span data-stu-id="87862-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="87862-110">Valitse **lisää** ja valitse sitten **OK.**</span><span class="sxs-lookup"><span data-stu-id="87862-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="87862-111">Kun olet valmis, valitse **Tallenna.**</span><span class="sxs-lookup"><span data-stu-id="87862-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="87862-112">Lisätietoja on Office [365:n Microsoft Defenderin turvallisten liitteiden ohjeissa.](https://go.microsoft.com/fwlink/?linkid=2092213)</span><span class="sxs-lookup"><span data-stu-id="87862-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
