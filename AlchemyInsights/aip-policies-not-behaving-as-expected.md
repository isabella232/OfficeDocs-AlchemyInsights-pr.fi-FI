---
title: 'AIP: Käytännöt eivät toimi odotetusti'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7926ff9ebbd54969fb5b3ae5d909baffe96a4292
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493023"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="4a42d-102">AIP: Käytännöt eivät toimi odotetusti</span><span class="sxs-lookup"><span data-stu-id="4a42d-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="4a42d-103">Azure-tietojen suojaus: Käytännöt eivät toimi odotetulla tavalla, katso seuraavat suositellut ohjeet eri käytäntöon liittyville kysymyksille:</span><span class="sxs-lookup"><span data-stu-id="4a42d-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="4a42d-104">Jos sinulla on ongelmia visuaalisten merkintöjen kanssa, tutustu [kun visuaalisia merkintöjä käytetään](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="4a42d-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="4a42d-105">Jos automaattisessa merkintöjen yhteydessä on ongelmia, tutustu [azure-tietojen suojauksen automaattisen ja suositellun luokituksen ehtojen määrittämiseen](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ja [mitä arkaluonteiset tietotyypit etsivät](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="4a42d-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>
3. <span data-ttu-id="4a42d-106">Jos sinulla on ongelmia Native/Pfile-suojauksen kanssa, tutustu [Tiedoston API-kokoonpanoon](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="4a42d-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="4a42d-107">Tarkista, käytätkö vaikutusaluekäytäntöjä, joita ei ole määritetty oikein: [Azure Information Protection -käytännön määrittäminen tietyille käyttäjille vaikutusaluekäytäntöjen avulla](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="4a42d-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="4a42d-108">Jos automaattinen merkintä ei toimi Outlookissa, kun liität merkittyä asiakirjaa, varmista, että DRMEncryptProperty-tiedostoa ei ole määritetty tässä kuvatulla tavalla: [IRM-rekisteriasetukset suojausta varten](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="4a42d-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="4a42d-109">Jos ongelmat jatkuvat, kerää Azure Information Protection -asiakaslokit ja liitä viedyt lokit tähän lippuun.</span><span class="sxs-lookup"><span data-stu-id="4a42d-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="4a42d-110">Avaa Office-asiakirja tai luo uusi sähköposti Outlookissa.</span><span class="sxs-lookup"><span data-stu-id="4a42d-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="4a42d-111">Valitse **Suojaa/herkkyys**  >  **-ohje ja -palaute**.</span><span class="sxs-lookup"><span data-stu-id="4a42d-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="4a42d-112">Valitse **Vie lokit**.</span><span class="sxs-lookup"><span data-stu-id="4a42d-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="4a42d-113">Tallenna lokit haluamaasi sijaintiin ja liitä ne tähän palvelupyyntöön.</span><span class="sxs-lookup"><span data-stu-id="4a42d-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="4a42d-114">Lisäresursseja:</span><span class="sxs-lookup"><span data-stu-id="4a42d-114">Additional resources:</span></span>

- [<span data-ttu-id="4a42d-115">Visual information protection -merkintöjen otsikon määrittäminen</span><span class="sxs-lookup"><span data-stu-id="4a42d-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="4a42d-116">Azure Information Protection -dokumentaation tarkasteleminen</span><span class="sxs-lookup"><span data-stu-id="4a42d-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="4a42d-117">Herkkyystarrojen käyttäminen Office-sovelluksissa</span><span class="sxs-lookup"><span data-stu-id="4a42d-117">Use sensitivity labels in Office apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

