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
ms.openlocfilehash: 72dc88a55b55954f34c95fa5b5038f472261c5bb
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758425"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="7042b-102">Herkkyysotsikot eivät näy</span><span class="sxs-lookup"><span data-stu-id="7042b-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="7042b-103">Herkkyysotsikoiden avulla voit luokitella ja suojata arkaluonteista sisältöäsi.</span><span class="sxs-lookup"><span data-stu-id="7042b-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="7042b-104">Ne voidaan luoda Microsoft 365 -yhteensopivuuskeskuksessa, Microsoft 365 -tietoturvakeskuksessa tai Microsoft 365-tietoturva-& yhteensopivuuskeskuksessa Luokitus- > Herkkyysotsikot-kohdassa.</span><span class="sxs-lookup"><span data-stu-id="7042b-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="7042b-105">Lisätietoja tästä ominaisuudesta on [ohjeaiheessa Herkkyysotsikoiden yleiskatsaus](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="7042b-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).</span></span>

<span data-ttu-id="7042b-106">Jos olet määrittänyt herkkyystunnisteet, mutta ne eivät näy Office-sovelluksissa, tarkista seuraavat asiat:</span><span class="sxs-lookup"><span data-stu-id="7042b-106">If you configured your sensitivity labels but they aren't appearing in the Office apps, check the following:</span></span>

- <span data-ttu-id="7042b-107">Varmista, että herkkyysotsikko on [julkaistu](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) haluamillesi käyttäjille ja ryhmille.</span><span class="sxs-lookup"><span data-stu-id="7042b-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="7042b-108">Varmista, että käyttäjä käyttää sovellusta, joka tukee herkkyystarroja - katso [asiakirjan herkkyysotsikot](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="7042b-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="7042b-109">Jos [siirrät Azure Information Protection -tunnisteita,](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)ota huomioon [tässä](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)luetellut seikat.</span><span class="sxs-lookup"><span data-stu-id="7042b-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="7042b-110">Tietojen menetyksen estämisen (DLP) tuki: Tällä hetkellä vain säilytysmerkintöjä voidaan käyttää ehtona DLP-käytännöissä.</span><span class="sxs-lookup"><span data-stu-id="7042b-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="7042b-111">DLP-käytännön herkkyysmerkintöjen tuki ei ole vielä käytettävissä, mutta työstämme sitä.</span><span class="sxs-lookup"><span data-stu-id="7042b-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="7042b-112">Kun salaus on käytössä herkkyystarrassa, voit valita joko seuraavista:</span><span class="sxs-lookup"><span data-stu-id="7042b-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="7042b-113">Käyttöoikeuksien määrittäminen nyt</span><span class="sxs-lookup"><span data-stu-id="7042b-113">Assign permissions now</span></span>
    - <span data-ttu-id="7042b-114">Anna käyttäjien määrittää käyttöoikeudet</span><span class="sxs-lookup"><span data-stu-id="7042b-114">Let users assign permissions</span></span>


<span data-ttu-id="7042b-115">Lisätietoja mahdollisista ongelmista on [ohjeaiheessa Arkaluonteisissa selityksissä tunnetut ongelmat](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span><span class="sxs-lookup"><span data-stu-id="7042b-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>