---
title: DLP-käytäntövihjeet eivät toimi
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 8a3b8175c077b77d1c9b5d859012faddcb1fa3a0
ms.sourcegitcommit: 099704f7f4bdf122d09bb4f7cc71d36fc77a7fcf
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2021
ms.locfileid: "51958699"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="2999f-102">DLP-käytäntövihjeen ongelmat</span><span class="sxs-lookup"><span data-stu-id="2999f-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="2999f-103">**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="2999f-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="2999f-104">Voit määrittää DLP-käytännön käytäntövihjeet tietoturva- &-yhteensopivuuskeskuksessa täydessä pakotustilassa seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="2999f-104">To configure policy tips on your DLP policy in the Security & Compliance center in full enforcement mode, do the following:</span></span>

- <span data-ttu-id="2999f-105">Varmista, että **käytäntövihjeet** on otettu käyttöön DLP-säännössä.</span><span class="sxs-lookup"><span data-stu-id="2999f-105">Ensure policy tips have been **enabled** on the DLP rule.</span></span> <span data-ttu-id="2999f-106">Ohjeet ovat kohdassa [Sähköposti-ilmoitusten lähettäminen ja käytäntövihjeiden näyttäminen DLP-käytäntöjä varten.](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="2999f-106">For steps, see [Send email notifications and show policy tips for DLP policies](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="2999f-107">Varmista, että sisältö vastaa sitä, mitä vaaditaan, jotta luottamuksellisten tietotyypin määritysten sääntö [voidaan ottaa käyttöön.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="2999f-107">Ensure your content matches what is required to trigger the rule outlined in [Sensitive information type entity definitions](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="2999f-108">Käytäntövihjeet näkyvät sekä OWA:ssa että Outlookissa.</span><span class="sxs-lookup"><span data-stu-id="2999f-108">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="2999f-109">Outlook 2013:a tai uudempaa versiota käytettäessä käytäntövihjeet näytetään kuitenkin vain tietyissä tilanteissa.</span><span class="sxs-lookup"><span data-stu-id="2999f-109">However, when using Outlook 2013 or later, policy tips are displayed only under certain conditions.</span></span> <span data-ttu-id="2999f-110">Jos haluat nähdä tietyn ehdon luettelon, katso käytäntövihjeiden näyttäminen [Outlook 2013:n tai uudemman sovelluksen tukemat ehdot.](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="2999f-110">For the specific conditions list, see [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

<span data-ttu-id="2999f-111">Lisätietoja DLP-käytäntövihjeistä on [DLP-käytäntövihjeiden](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) ohjeissa ja [tukimatriisissa.](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps)</span><span class="sxs-lookup"><span data-stu-id="2999f-111">For information on DLP Policy tips, see [DLP Policy Tips Reference](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) and [Support Matrix for DLP Policy tips](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps).</span></span>