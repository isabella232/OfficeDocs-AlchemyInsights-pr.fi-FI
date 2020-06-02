---
title: Herkkyysotsikot eivät näy
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 1326eca02044014a8e9c072fcc3e4cd3a41c7a9f
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511649"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="bede2-102">Herkkyysotsikot eivät näy</span><span class="sxs-lookup"><span data-stu-id="bede2-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="bede2-103">Herkkyystarrojen avulla voit luokitella ja suojata arkaluonteista sisältöäsi.</span><span class="sxs-lookup"><span data-stu-id="bede2-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="bede2-104">Ne voidaan luoda Microsoft 365 -yhteensopivuuskeskuksessa, Microsoft 365-tietoturvakeskuksessa tai Microsoft 365:n tietoturvakeskus & Compliance Centerissä kohdassa Luokittelu > Herkkyysetsaaminen.</span><span class="sxs-lookup"><span data-stu-id="bede2-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="bede2-105">Lisätietoja tästä ominaisuudesta on [ohjeaiheessa Herkkyystarrojen yleiskatsaus](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="bede2-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span></span>

<span data-ttu-id="bede2-106">Jos olet määrittänyt herkkyystarrat, mutta ne eivät näy Office-sovelluksissa, tarkista seuraavat asiat:</span><span class="sxs-lookup"><span data-stu-id="bede2-106">If you configured your sensitivity labels but they aren't appearing in the Office apps, check the following:</span></span>

- <span data-ttu-id="bede2-107">Varmista, että herkkyysotsikko on [julkaistu](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) haluamillesi käyttäjille ja ryhmille.</span><span class="sxs-lookup"><span data-stu-id="bede2-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="bede2-108">Varmista, että käyttäjä käyttää herkkyystarroja tukevaa sovellusta - katso [asiakirjan herkkyysotsikot](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="bede2-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="bede2-109">Jos siirrät [Azure Information Protection -tunnisteita,](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)ota huomioon [tässä](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)luetellut seikat .</span><span class="sxs-lookup"><span data-stu-id="bede2-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="bede2-110">Tietojen menetyksen estäminen (DLP) -tuki: Tällä hetkellä vain säilytysmerkintöjä voidaan käyttää ehtona DLP-käytännöissä.</span><span class="sxs-lookup"><span data-stu-id="bede2-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="bede2-111">DLP-käytännön herkkyysmerkintöjen tuki ei ole vielä käytettävissä, mutta työstämme sitä parhaillaan.</span><span class="sxs-lookup"><span data-stu-id="bede2-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="bede2-112">Kun salaus on käytössä herkkyysotsikko, voit valita joko:</span><span class="sxs-lookup"><span data-stu-id="bede2-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="bede2-113">Käyttöoikeuksien määrittäminen nyt</span><span class="sxs-lookup"><span data-stu-id="bede2-113">Assign permissions now</span></span>
    - <span data-ttu-id="bede2-114">Salli käyttäjien määrittää käyttöoikeudet</span><span class="sxs-lookup"><span data-stu-id="bede2-114">Let users assign permissions</span></span>


<span data-ttu-id="bede2-115">Lisätietoja mahdollisista ongelmista on kohdassa [Tunnetut herkkyystarroihin liittyvät ongelmat](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span><span class="sxs-lookup"><span data-stu-id="bede2-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>