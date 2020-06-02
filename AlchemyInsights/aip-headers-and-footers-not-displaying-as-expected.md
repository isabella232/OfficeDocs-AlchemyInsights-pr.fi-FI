---
title: 'AIP: Ylä- ja alatunnisteet eivät näy odotetulla tavalla'
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
- "4541"
ms.openlocfilehash: 418362beea221a7cb9d8fd4be6cfc0f28022093d
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/26/2020
ms.locfileid: "44493018"
---
# <a name="aip-headers-and-footers-not-displaying-as-expected"></a><span data-ttu-id="81ce7-102">AIP: Ylä- ja alatunnisteet eivät näy odotetulla tavalla</span><span class="sxs-lookup"><span data-stu-id="81ce7-102">AIP: Headers and footers not displaying as expected</span></span>

<span data-ttu-id="81ce7-103">Jos visuaalisissa merkinnöissä ilmenee ongelmia, jotka eivät näy odotetulla tavalla, tarkastele seuraavia ohjeita:</span><span class="sxs-lookup"><span data-stu-id="81ce7-103">If you are experiencing issues with visual markings not displaying as expected, view the following guidelines:</span></span>

1. <span data-ttu-id="81ce7-104">Varmista, että olet tarkistanut [Kun visuaalisia merkintöjä käytetään](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="81ce7-104">Make sure you have reviewed [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="81ce7-105">Tarkista Office-merkinnöissä, [kun Office 365 käyttää sisällön merkintää ja salausta](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption).</span><span class="sxs-lookup"><span data-stu-id="81ce7-105">For Office labeling, review [When Office 365 applies content marking and encryption](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps#when-office-apps-apply-content-marking-and-encryption).</span></span>
3. <span data-ttu-id="81ce7-106">Jos haluat poistaa aiemmin luodut ylä- ja alatunnisteet, tarkista [Poista ylä- ja alatunnisteet muista merkintäratkaisuista](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions).</span><span class="sxs-lookup"><span data-stu-id="81ce7-106">If you want to remove existing headers/footers, review [Remove headers and footers from other labeling solutions](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-customizations#remove-headers-and-footers-from-other-labeling-solutions).</span></span>

<span data-ttu-id="81ce7-107">Jos ongelma ei poistu, kerää Azure Information Protection -asiakaslokit ja liitä viedyt lokit tähän lippuun.</span><span class="sxs-lookup"><span data-stu-id="81ce7-107">If you are still experiencing the issue, collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

<span data-ttu-id="81ce7-108">**Azure-tietojen suojauslokien vieminen**</span><span class="sxs-lookup"><span data-stu-id="81ce7-108">**Export Azure Information Protection logs**</span></span>

1. <span data-ttu-id="81ce7-109">Avaa Office-asiakirja tai luo uusi sähköposti Outlookissa.</span><span class="sxs-lookup"><span data-stu-id="81ce7-109">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="81ce7-110">Valitse **Suojaa/herkkyys**  >  **-ohje ja -palaute**.</span><span class="sxs-lookup"><span data-stu-id="81ce7-110">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="81ce7-111">Valitse **Vie lokit**.</span><span class="sxs-lookup"><span data-stu-id="81ce7-111">Click **Export Logs**.</span></span>
4. <span data-ttu-id="81ce7-112">Tallenna lokit haluamaasi sijaintiin ja liitä ne tähän palvelupyyntöön.</span><span class="sxs-lookup"><span data-stu-id="81ce7-112">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="81ce7-113">Lisätietoja on seuraavissa ohjeissa:</span><span class="sxs-lookup"><span data-stu-id="81ce7-113">For additional information, see:</span></span>

- [<span data-ttu-id="81ce7-114">Visual information protection -merkintöjen otsikon määrittäminen</span><span class="sxs-lookup"><span data-stu-id="81ce7-114">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="81ce7-115">Azure Information Protection -dokumentaation tarkasteleminen</span><span class="sxs-lookup"><span data-stu-id="81ce7-115">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="81ce7-116">Azure-tietojen suojausta koskevat vaatimukset</span><span class="sxs-lookup"><span data-stu-id="81ce7-116">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="81ce7-117">Azure Information Protectionin pika-aloitusopas</span><span class="sxs-lookup"><span data-stu-id="81ce7-117">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [<span data-ttu-id="81ce7-118">Lataa Azure Information Protection -asiakasohjelma</span><span class="sxs-lookup"><span data-stu-id="81ce7-118">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
