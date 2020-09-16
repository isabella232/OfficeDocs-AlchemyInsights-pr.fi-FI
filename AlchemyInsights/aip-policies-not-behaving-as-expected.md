---
title: 'AIP: käytännöt, joita ei voi käyttäytyä odotusten mukaan'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663186"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="7c1b4-102">AIP: käytännöt, joita ei voi käyttäytyä odotusten mukaan</span><span class="sxs-lookup"><span data-stu-id="7c1b4-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="7c1b4-103">Azure Information Protectionin käytäntö: käytännöt, jotka eivät toimi oikein, saat ohjeita eri poliittisiin ongelmiin seuraavista ohjeista:</span><span class="sxs-lookup"><span data-stu-id="7c1b4-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="7c1b4-104">Jos sinulla on visuaalisia merkintöjä koskevia ongelmia, tarkista, [Milloin visuaalisia merkintöjä](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)käytetään.</span><span class="sxs-lookup"><span data-stu-id="7c1b4-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="7c1b4-105">Jos sinulla on automaattisia merkintöjä koskevia ongelmia, Tutustu siihen, [miten voit määrittää ehdot, jotka koskevat Azure Information Protectionin automaattista ja suositeltua luokittelua](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) ja [mitä arkaluonteiset tieto tyypit](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)etsivät.</span><span class="sxs-lookup"><span data-stu-id="7c1b4-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="7c1b4-106">Jos sinulla on ongelmia Native/pfile-suojauksen kanssa, tarkista [tiedoston API-määritys](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="7c1b4-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="7c1b4-107">Tarkista, käytätkö käytössä olevia käytäntöjä, joita ei ole määritetty oikein: [Azuren tietojen suojaus käytännön määrittäminen tietyille käyttäjille määritettyjen käytäntöjen avulla](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="7c1b4-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="7c1b4-108">Jos automaattinen merkintä ei toimi Outlookissa, kun kiinnität merkittyä asia kirjaa, varmista, että DRMEncryptProperty-ominaisuutta ei ole määritetty tässä kuvatulla tavalla: [tieto turvan hallinnan rekisteri asetukset](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="7c1b4-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="7c1b4-109">Jos kohtaat edelleen ongelmia, voit kerätä Azure Information Protectionin asiakas lokit ja liittää viedyt lokit tähän lipussa.</span><span class="sxs-lookup"><span data-stu-id="7c1b4-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="7c1b4-110">Avaa Office-tiedosto tai luo uusi Sähkö posti viesti Outlookissa.</span><span class="sxs-lookup"><span data-stu-id="7c1b4-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="7c1b4-111">Valitse **suojaa/herkkyys**-  >  **Ohje ja palaute**.</span><span class="sxs-lookup"><span data-stu-id="7c1b4-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="7c1b4-112">Valitse **Vie lokit**.</span><span class="sxs-lookup"><span data-stu-id="7c1b4-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="7c1b4-113">Tallenna lokit valitsemaasi sijaintiin ja liitä ne tähän palvelu pyyntöön.</span><span class="sxs-lookup"><span data-stu-id="7c1b4-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="7c1b4-114">Lisäresursseja:</span><span class="sxs-lookup"><span data-stu-id="7c1b4-114">Additional resources:</span></span>

- [<span data-ttu-id="7c1b4-115">Azure Information Protectionin visuaalisten merkintöjen otsikon määrittäminen</span><span class="sxs-lookup"><span data-stu-id="7c1b4-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="7c1b4-116">Azure Information Protectionin ohjeiden tarkasteleminen</span><span class="sxs-lookup"><span data-stu-id="7c1b4-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="7c1b4-117">Luottamuksellisuusmerkkien käyttäminen Microsoft 365-sovelluksissa</span><span class="sxs-lookup"><span data-stu-id="7c1b4-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

