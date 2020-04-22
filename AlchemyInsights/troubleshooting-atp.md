---
title: Office 365:n edistyneen uhkien suojauksen vianmääritys
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1039
ms.assetid: ''
ms.openlocfilehash: c90c8e9cb23cba93883cc1148fcbca77c9e92408
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732399"
---
# <a name="troubleshooting-office-365-advanced-threat-protection"></a><span data-ttu-id="0f101-102">Office 365:n edistyneen uhkien suojauksen vianmääritys</span><span class="sxs-lookup"><span data-stu-id="0f101-102">Troubleshooting Office 365 Advanced Threat Protection</span></span>

- <span data-ttu-id="0f101-103">Huomaatko viiveitä viestin toimittamisessa?</span><span class="sxs-lookup"><span data-stu-id="0f101-103">Do you notice delays in message delivery?</span></span> <span data-ttu-id="0f101-104">Käytä [ATP](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) Safe Attachments -käytännön Dynaaminen toimitus -vaihtoehtoa.</span><span class="sxs-lookup"><span data-stu-id="0f101-104">Use the [Dynamic Delivery](https://docs.microsoft.com/office365/securitycompliance/dynamic-delivery-and-previewing) option in your ATP Safe Attachments policy.</span></span> <span data-ttu-id="0f101-105">Tämä auttaa välttämään viestin viiveitä ja suojaa samalla vastaanottajia haitallisilta tiedostoilta.</span><span class="sxs-lookup"><span data-stu-id="0f101-105">This will help avoid message delays while protecting recipients from malicious files.</span></span>

- <span data-ttu-id="0f101-106">Haluatko ilmoittaa microsoftille vääriä positiivisia tai vääriä negatiivisia negatiivisia?</span><span class="sxs-lookup"><span data-stu-id="0f101-106">Do you want to report false positives or false negatives to Microsoft?</span></span> <span data-ttu-id="0f101-107">Tämän [linkin](https://www.microsoft.com/wdsi/filesubmission/) avulla voit lähettää tiedostoja analysoitavaksi.</span><span class="sxs-lookup"><span data-stu-id="0f101-107">Use this [link](https://www.microsoft.com/wdsi/filesubmission/) to submit files for analysis.</span></span>

- <span data-ttu-id="0f101-108">Tiesitkö, että voit ottaa safe links -suojauksen käyttöön organisaation vastaanottajien välillä lähetetyille sisäisille sähköpostiviesteille?</span><span class="sxs-lookup"><span data-stu-id="0f101-108">Did you know that you can enable Safe Links protection for internal email sent between recipients within your organization?</span></span> <span data-ttu-id="0f101-109">Toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="0f101-109">Follow these steps:</span></span>

  1. <span data-ttu-id="0f101-110">Siirry [https://protection.office.com](https://protection.office.com) yleiseen järjestelmänvalvojan tai suojauksen järjestelmänvalvojan tiliin ja kirjaudu sisään.</span><span class="sxs-lookup"><span data-stu-id="0f101-110">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

  2. <span data-ttu-id="0f101-111">Valitse vasemmanpuoleisen siirtymisruudun **Uhkien hallinta**-kohdassa **Käytännön** \> **turvalliset linkit**.</span><span class="sxs-lookup"><span data-stu-id="0f101-111">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Links**.</span></span>

  3. <span data-ttu-id="0f101-112">Valitse **käytäntö koko organisaatioon sovellettavissa käytännöissä** ja valitse **sitten Muokkaa**.</span><span class="sxs-lookup"><span data-stu-id="0f101-112">In the **Policies that apply to the entire organization** section, select the policy and click **Edit**.</span></span>

  4. <span data-ttu-id="0f101-113">Ota **Asetukset -kohdassa**käyttöön **Käytä turvallisia linkkejä organisaation sisällä lähetettyihin viesteihin**.</span><span class="sxs-lookup"><span data-stu-id="0f101-113">Under **Settings**, enable **Apply safe links to messages sent within the organization**.</span></span>
