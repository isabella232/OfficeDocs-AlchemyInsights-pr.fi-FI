---
title: 'AIP: Käytännöt eivät toimi odotetulla tavalla'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821624"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="8a76a-102">AIP: Käytännöt eivät toimi odotetulla tavalla</span><span class="sxs-lookup"><span data-stu-id="8a76a-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="8a76a-103">Azure Information Protection: Käytännöt eivät toimi odotetulla tavalla, katso seuraavista ohjeista eri käytäntöihin liittyviä ohjeita:</span><span class="sxs-lookup"><span data-stu-id="8a76a-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="8a76a-104">Jos visuaalisissa merkinnöissä on ongelmia, lue kohta [Kun visuaalisia merkintöjä käytetään](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="8a76a-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="8a76a-105">Jos sinulla on ongelmia automaattisen otsikoinnin kanssa, lue ohjeet automaattisen ja suosittelun luokittelun määrittämiseen [Azure Information Protectionille](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ja Mitä luottamukselliset [tietotyypit etsivät](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="8a76a-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="8a76a-106">Jos sinulla on ongelmia alkuperäisen/Pfile-suojauksen kanssa, tarkista Tiedoston [ohjelmointirajapinnan määritykset.](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)</span><span class="sxs-lookup"><span data-stu-id="8a76a-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="8a76a-107">Tarkista, käytätkö kohdistettuja käytäntöjä, joita ei ole määritetty oikein: [Azure Information Protection -käytännön määrittäminen tietyille käyttäjille kohdistettujen käytäntöjen avulla](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="8a76a-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="8a76a-108">Jos automaattinen selite ei toimi Outlookissa, kun liität tunnisteen, varmista, että DRMEncryptProperty-funktiota ei ole määritetty seuraavassa kuvatulla tavalla: [IRM-rekisteriasetukset suojauksen varmistamiseksi.](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)</span><span class="sxs-lookup"><span data-stu-id="8a76a-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="8a76a-109">Jos ongelmia ilmenee edelleen, kerää Azure Information Protection -asiakaslokit ja liitä viedyt lokit tähän lippuun.</span><span class="sxs-lookup"><span data-stu-id="8a76a-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="8a76a-110">Avaa Office-tiedosto tai luo uusi sähköpostiviesti Outlookissa.</span><span class="sxs-lookup"><span data-stu-id="8a76a-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="8a76a-111">Valitse **Suojaus ja luottamuksellisuus** > **Ohje- ja palaute**.</span><span class="sxs-lookup"><span data-stu-id="8a76a-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="8a76a-112">Valitse **Vie lokit**.</span><span class="sxs-lookup"><span data-stu-id="8a76a-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="8a76a-113">Tallenna lokit sijaintisi mukaan ja liitä ne tähän palvelupyyntöön.</span><span class="sxs-lookup"><span data-stu-id="8a76a-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="8a76a-114">Lisäresursseja:</span><span class="sxs-lookup"><span data-stu-id="8a76a-114">Additional resources:</span></span>

- [<span data-ttu-id="8a76a-115">Otsikon määrittäminen visuaalisia merkintöjä varten Azure Information Protectionissa</span><span class="sxs-lookup"><span data-stu-id="8a76a-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="8a76a-116">Tutustu Azure Information Protection -ohjeisiin</span><span class="sxs-lookup"><span data-stu-id="8a76a-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="8a76a-117">Luottamuksellisuusmerkkien käyttäminen Microsoft 365 -sovelluksissa</span><span class="sxs-lookup"><span data-stu-id="8a76a-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

