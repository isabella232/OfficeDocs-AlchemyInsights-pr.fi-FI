---
title: 'AIP-skanneri: asennus ja määritys'
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
- "9002278"
- "5119"
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821660"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="2e60d-102">AIP-skanneri: asennus ja määritys</span><span class="sxs-lookup"><span data-stu-id="2e60d-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="2e60d-103">**Asenna AIP-skanneri noudattamalla suositeltuja ohjeita:**</span><span class="sxs-lookup"><span data-stu-id="2e60d-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="2e60d-104">Jos päivität ja et suorita puhdasta asennusta, varmista, että olet noudattanut [Ohjeita Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) -skannerin päivittämiseen ja yhdistetyn osoitetarrasovelluksen päivittämiseen, katso Azure Information Protection [-skannerin päivittäminen.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)</span><span class="sxs-lookup"><span data-stu-id="2e60d-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="2e60d-105">Varmista, että noudatat kaikkia [palomuurien ja verkkoinfrastruktuurin asetusten vaatimuksia.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)</span><span class="sxs-lookup"><span data-stu-id="2e60d-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="2e60d-106">Varmista, että [käytäntöihin on](https://docs.microsoft.com/azure/information-protection/configure-policy) määritetty automaattinen selite tai että käytäntö sisältää oletusotsikot.</span><span class="sxs-lookup"><span data-stu-id="2e60d-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="2e60d-107">Varmista, että asianmukainen tiedostotyyppi on määritetty selite-/suojausta varten artikkelissa Azure Information Protection -asiakasohjelman tukemat [tiedostotyypit kuvatulla tavalla.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)</span><span class="sxs-lookup"><span data-stu-id="2e60d-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="2e60d-108">Jos haluat muuttaa oletusasetuksia, noudata seuraavia ohjeita: [Tiedostojen oletussuojaustason muuttaminen.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)</span><span class="sxs-lookup"><span data-stu-id="2e60d-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="2e60d-109">Varmista, että skanneripalvelun suorittamiseen määritetyllä käyttäjätilillä on oikeus käyttää kaikkia määritettyjä säilöjä.</span><span class="sxs-lookup"><span data-stu-id="2e60d-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="2e60d-110">Jos ongelmia ilmenee edelleen, vie skannerilokit ja lisää ne tukipalveluun.</span><span class="sxs-lookup"><span data-stu-id="2e60d-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="2e60d-111">**Azure Information Protection Scanner -lokien vieminen**</span><span class="sxs-lookup"><span data-stu-id="2e60d-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="2e60d-112">Siirry kohtaan %localappdata%\Microsoft\MSIP skanneripalvelun suorittaman käyttäjäkontekstin mukaisesti.</span><span class="sxs-lookup"><span data-stu-id="2e60d-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="2e60d-113">Pakkaa kaikki MSIP-kansion sisältö.</span><span class="sxs-lookup"><span data-stu-id="2e60d-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="2e60d-114">Tallenna lokit haluamaasi sijaintiin ja liitä ne palvelupyyntöösi.</span><span class="sxs-lookup"><span data-stu-id="2e60d-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="2e60d-115">Voit käyttää myös [Export-AIPLogs -OnBehalfOf-sovellusta.](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)</span><span class="sxs-lookup"><span data-stu-id="2e60d-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="2e60d-116">**Lisätietoja on kohdassa:**</span><span class="sxs-lookup"><span data-stu-id="2e60d-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="2e60d-117">Azure Information Protection -skannerin käyttöönotto tiedostojen automaattista luokittelemista ja suojaamista varten</span><span class="sxs-lookup"><span data-stu-id="2e60d-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="2e60d-118">Set-AIPAuthentication-parametrin määritäminen ja käyttö</span><span class="sxs-lookup"><span data-stu-id="2e60d-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="2e60d-119">Suorita etsintäjakso ja tarkastele skannerin raportteja</span><span class="sxs-lookup"><span data-stu-id="2e60d-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="2e60d-120">Tutustu Azure Information Protection -ohjeisiin</span><span class="sxs-lookup"><span data-stu-id="2e60d-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="2e60d-121">Azure Information Protectionin vaatimukset</span><span class="sxs-lookup"><span data-stu-id="2e60d-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="2e60d-122">Lataa Azure Information Protection -asiakasohjelma</span><span class="sxs-lookup"><span data-stu-id="2e60d-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
