---
title: Herkkyys Tunnisteet eivät ilmesity
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801181"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="f30fe-102">Herkkyys Tunnisteet eivät ilmesity</span><span class="sxs-lookup"><span data-stu-id="f30fe-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="f30fe-103">Herkkyys merkintöjen avulla voit luokitella ja suojata arkaluontoista sisältöä.</span><span class="sxs-lookup"><span data-stu-id="f30fe-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="f30fe-104">Ne voidaan luoda Microsoft 365-yhteensopivuus keskuksessa, Microsoft 365-tieto turva keskuksessa tai Microsoft 365-tieto turva & yhteensopivuus keskuksessa luokittelu > herkkyys-selitteissä.</span><span class="sxs-lookup"><span data-stu-id="f30fe-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="f30fe-105">Lisä tietoja tästä ominaisuudesta on artikkelissa [herkkyys merkkien yleiskatsaus](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="f30fe-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span></span>

<span data-ttu-id="f30fe-106">Jos olet määrittänyt luottamuksellisuustunnisteet, mutta ne eivät näy Microsoft 365-sovelluksissa, tarkista seuraavat asiat:</span><span class="sxs-lookup"><span data-stu-id="f30fe-106">If you configured your sensitivity labels but they aren't appearing in the Microsoft 365 apps, check the following:</span></span>

- <span data-ttu-id="f30fe-107">Varmista, että luottamuksellisuustarra on [julkaistu](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) käyttäjille ja ryhmille, jotka haluat määrittää.</span><span class="sxs-lookup"><span data-stu-id="f30fe-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="f30fe-108">Varmista, että käyttäjä käyttää sovellusta, joka tukee herkkyys otsikoita-Katso [asia kirjan herkkyys otsikoita](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="f30fe-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="f30fe-109">Jos olet [siirtämässä Azure-tieto turva-otsikoita](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), ota huomioon [tässä](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)luetellut seikat.</span><span class="sxs-lookup"><span data-stu-id="f30fe-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="f30fe-110">Tietojen menetyksen estämisen (DLP) tuki: tällä hetkellä DLP-käytäntöjen ehtona voidaan käyttää vain säilytys otsikoita.</span><span class="sxs-lookup"><span data-stu-id="f30fe-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="f30fe-111">DLP-käytäntöjen luottamuksellisuusmerkintöjen tuki ei ole vielä käytettävissä, mutta työskentelemme sen parissa.</span><span class="sxs-lookup"><span data-stu-id="f30fe-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="f30fe-112">Kun salaus on otettu käyttöön luottamuksellisuustarrassa, voit valita jommankumman seuraavista:</span><span class="sxs-lookup"><span data-stu-id="f30fe-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="f30fe-113">Määritä käyttö oikeudet nyt</span><span class="sxs-lookup"><span data-stu-id="f30fe-113">Assign permissions now</span></span>
    - <span data-ttu-id="f30fe-114">Salli käyttäjien määrittää käyttö oikeuksia</span><span class="sxs-lookup"><span data-stu-id="f30fe-114">Let users assign permissions</span></span>


<span data-ttu-id="f30fe-115">Lisä tietoja mahdollisista ongelmista on kohdassa [arkaluonteisiin tunniste tietoihin liittyvät tunnetut ongelmat](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span><span class="sxs-lookup"><span data-stu-id="f30fe-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>