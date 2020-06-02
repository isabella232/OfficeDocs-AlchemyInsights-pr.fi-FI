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
ms.openlocfilehash: 527556fcb02525eb88ea992c38a2ddfcba6f9453
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506555"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="e2c15-102">AIP: Käytännöt eivät toimi odotetusti</span><span class="sxs-lookup"><span data-stu-id="e2c15-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="e2c15-103">Azure-tietojen suojaus: Käytännöt eivät toimi odotetulla tavalla, katso seuraavat suositellut ohjeet eri käytäntöon liittyville kysymyksille:</span><span class="sxs-lookup"><span data-stu-id="e2c15-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="e2c15-104">Jos sinulla on ongelmia visuaalisten merkintöjen kanssa, tutustu [kun visuaalisia merkintöjä käytetään](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="e2c15-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="e2c15-105">Jos automaattisessa merkintöjen yhteydessä on ongelmia, tutustu [azure-tietojen suojauksen automaattisen ja suositellun luokituksen ehtojen määrittämiseen](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ja [mitä arkaluonteiset tietotyypit etsivät](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="e2c15-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="e2c15-106">Jos sinulla on ongelmia Native/Pfile-suojauksen kanssa, tutustu [Tiedoston API-kokoonpanoon](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="e2c15-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="e2c15-107">Tarkista, käytätkö vaikutusaluekäytäntöjä, joita ei ole määritetty oikein: [Azure Information Protection -käytännön määrittäminen tietyille käyttäjille vaikutusaluekäytäntöjen avulla](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="e2c15-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="e2c15-108">Jos automaattinen merkintä ei toimi Outlookissa, kun liität merkittyä asiakirjaa, varmista, että DRMEncryptProperty-tiedostoa ei ole määritetty tässä kuvatulla tavalla: [IRM-rekisteriasetukset suojausta varten](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="e2c15-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="e2c15-109">Jos ongelmat jatkuvat, kerää Azure Information Protection -asiakaslokit ja liitä viedyt lokit tähän lippuun.</span><span class="sxs-lookup"><span data-stu-id="e2c15-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="e2c15-110">Avaa Office-asiakirja tai luo uusi sähköposti Outlookissa.</span><span class="sxs-lookup"><span data-stu-id="e2c15-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="e2c15-111">Valitse **Suojaa/herkkyys**  >  **-ohje ja -palaute**.</span><span class="sxs-lookup"><span data-stu-id="e2c15-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="e2c15-112">Valitse **Vie lokit**.</span><span class="sxs-lookup"><span data-stu-id="e2c15-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="e2c15-113">Tallenna lokit haluamaasi sijaintiin ja liitä ne tähän palvelupyyntöön.</span><span class="sxs-lookup"><span data-stu-id="e2c15-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="e2c15-114">Lisäresursseja:</span><span class="sxs-lookup"><span data-stu-id="e2c15-114">Additional resources:</span></span>

- [<span data-ttu-id="e2c15-115">Visual information protection -merkintöjen otsikon määrittäminen</span><span class="sxs-lookup"><span data-stu-id="e2c15-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="e2c15-116">Azure Information Protection -dokumentaation tarkasteleminen</span><span class="sxs-lookup"><span data-stu-id="e2c15-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="e2c15-117">Herkkyystarrojen käyttäminen Office-sovelluksissa</span><span class="sxs-lookup"><span data-stu-id="e2c15-117">Use sensitivity labels in Office apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

