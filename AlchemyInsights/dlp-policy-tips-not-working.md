---
title: DLP-käytäntöjen vihjeet eivät toimi
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
ms.openlocfilehash: 1e1f9b84cb8bd07468d3da0eeaff3716b9a309a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679582"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="d19aa-102">DLP-käytäntöjen kärjen ongelmat</span><span class="sxs-lookup"><span data-stu-id="d19aa-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="d19aa-103">**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="d19aa-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="d19aa-104">**DLP-käytäntöjen vinkit**</span><span class="sxs-lookup"><span data-stu-id="d19aa-104">**DLP policy tips**</span></span>

<span data-ttu-id="d19aa-105">**DLP-käytäntöjä**käytettäessä käyttäjät voivat saada ilmoituksen käytäntö rikkomuksesta, jossa on **käytäntö vihjeitä**.</span><span class="sxs-lookup"><span data-stu-id="d19aa-105">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="d19aa-106">Järjestelmänvalvojat voivat määrittää käytäntöä koskevia vihjeitä, jotka näytetään, kun ne testaavat DLP-käytäntöään tai kun käytännöt ovat täydessä pakotus tilassa.</span><span class="sxs-lookup"><span data-stu-id="d19aa-106">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="d19aa-107">Jos haluat määrittää DLP-käytännölle toimintapoliittisia vihjeitä tieto turva-ja yhteensopivuus keskuksessa koko pakotus tilassa, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="d19aa-107">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="d19aa-108">Varmista, että käytäntöjen vihjeet on **otettu käyttöön** DLP-säännössä noudattamalla [tässä](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)annettuja ohjeita.</span><span class="sxs-lookup"><span data-stu-id="d19aa-108">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="d19aa-109">Varmista, että **sisältö vastaa** sitä, mitä [tässä artikkelissa](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)hahmoteltu sääntö **edellyttää** .</span><span class="sxs-lookup"><span data-stu-id="d19aa-109">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="d19aa-110">Käytäntöjen vihjeet näkyvät sekä OWA-sovelluksessa että Outlookissa.</span><span class="sxs-lookup"><span data-stu-id="d19aa-110">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="d19aa-111">Kun käytät **Outlook 2013 tai uudempaa versiota**, käytäntöjen vihjeet näkyvät kuitenkin vain tietyissä tilanteissa.</span><span class="sxs-lookup"><span data-stu-id="d19aa-111">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="d19aa-112">Nämä ehdot on lueteltu tässä: [Outlook 2013 tai sitä uudemman version tukemat ehdot käytäntöjen vihjeiden näyttämiseksi](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="d19aa-112">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span></span>

<span data-ttu-id="d19aa-113">Lisä tietoja DLP-käytäntö vihjeistä on Ohje aiheissa: [käytännön vihjeiden näyttäminen DLP-käytäntöjä varten](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="d19aa-113">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)</span></span>
  