---
title: Herkkyys merkinnät eivät näy
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 4bf8e02246c966f22648467386a7862f0521fecf
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207222"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="7c464-102">Herkkyys merkinnät eivät näy</span><span class="sxs-lookup"><span data-stu-id="7c464-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="7c464-103">Herkkyys tunnisteiden avulla voit luokitella arkaluontoista sisältöä ja suojata sen.</span><span class="sxs-lookup"><span data-stu-id="7c464-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="7c464-104">Ne voidaan luoda Microsoft 365 Compliance Centerissä, Microsoft 365 tieto turva keskuksessa tai Office 365 Security & Compliance Centerissa luokittelu > herkkyys merkintöjen alla.</span><span class="sxs-lookup"><span data-stu-id="7c464-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Office 365 Security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="7c464-105">Lisä tietoja tästä ominaisuudesta on kohdassa [herkkyys merkintöjen yleiskuvaus](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="7c464-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).</span></span>

<span data-ttu-id="7c464-106">Jos olet määrittänyt herkkyys Tunnisteet, mutta ne eivät näy Office-sovelluksissa, tarkista seuraavat seikat:</span><span class="sxs-lookup"><span data-stu-id="7c464-106">If you configured your sensitivity labels but they aren't appearing in the Office apps, check the following:</span></span>

- <span data-ttu-id="7c464-107">Varmista, että herkkyys tarra on [julkaistu](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) haluamilleen käyttäjille ja ryhmille.</span><span class="sxs-lookup"><span data-stu-id="7c464-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="7c464-108">Varmista, että käyttäjä käyttää sovellusta, joka tukee herkkyys tarroja – Katso [asia kirjan herkkyys tarrat](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="7c464-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).</span></span>

- <span data-ttu-id="7c464-109">Jos olet [siirtamassa Azure Information Protection-tunnisteita](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), Huomaa [tässä](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)luetellut seikat.</span><span class="sxs-lookup"><span data-stu-id="7c464-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="7c464-110">Tietojen menetyksen estämisen (DLP) tuki: tällä hetkellä vain säilytys tarroja voidaan käyttää ehtona DLP-käytännöissä.</span><span class="sxs-lookup"><span data-stu-id="7c464-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="7c464-111">DLP-käytännön herkkyys merkintöjen tuki ei ole vielä saatavilla, mutta työskentelemme sen parissa.</span><span class="sxs-lookup"><span data-stu-id="7c464-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="7c464-112">Kun salaus on otettu käyttöön herkkyys merkinnässä, voit valita joko:</span><span class="sxs-lookup"><span data-stu-id="7c464-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="7c464-113">Määritä käyttö oikeudet nyt</span><span class="sxs-lookup"><span data-stu-id="7c464-113">Assign permissions now</span></span>
    - <span data-ttu-id="7c464-114">Anna käyttäjien määrittää käyttö oikeuksia</span><span class="sxs-lookup"><span data-stu-id="7c464-114">Let users assign permissions</span></span>


<span data-ttu-id="7c464-115">Lisä tietoja mahdollisista ongelmista [on aiheessa herkkyys otsikoihin liittyvät tunnetut ongelmat](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span><span class="sxs-lookup"><span data-stu-id="7c464-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>