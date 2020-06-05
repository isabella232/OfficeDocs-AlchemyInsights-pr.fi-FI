---
title: AIP-tunnistekäytäntöjen luominen
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569200"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="62978-102">AIP-tunnistekäytäntöjen luominen</span><span class="sxs-lookup"><span data-stu-id="62978-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="62978-103">Azure Information Protection (AIP) -tunnisteita voidaan käyttää kaikkien tietojen kanssa, joita organisaatio yleensä luo ja tallentaa pienimmästä henkilötietojen luokittelusta erittäin luottamuksellisten tietojen korkeimpaan luokitteluun.</span><span class="sxs-lookup"><span data-stu-id="62978-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="62978-104">Azure Information Protection -käytännöt koskevat Azure Information Protection (AIP) classic -asiakasta eikä [AIP Unified Labeling -asiakasohjelmaa.](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history)</span><span class="sxs-lookup"><span data-stu-id="62978-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="62978-105">Voit määrittää useita elementtejä AIP-käytännössä, mukaan lukien seuraavat vaihtoehdot:</span><span class="sxs-lookup"><span data-stu-id="62978-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="62978-106">Vaihtoehto, jonka otsikko antaa järjestelmänvalvojille tai käyttäjälle luokitella ja suojata (valinnainen) asiakirjoja ja sähköposteja</span><span class="sxs-lookup"><span data-stu-id="62978-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="62978-107">Mahdollisuus pakottaa luokittelu, kun käyttäjät tallentavat asiakirjoja ja lähettävät sähköpostia</span><span class="sxs-lookup"><span data-stu-id="62978-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="62978-108">Mahdollisuus merkitä automaattisesti sähköpostiviesti liitteiden perusteella.</span><span class="sxs-lookup"><span data-stu-id="62978-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="62978-109">Mahdollisuus määrittää, näytetäänkö tietojen suojauspalkki Office-sovelluksissa</span><span class="sxs-lookup"><span data-stu-id="62978-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="62978-110">Lisätietoja Azure-tietojen suojauskäytännöistä on kohdassa Azure [Information Protection -käytännön yleiskatsaus](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="62978-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="62978-111">Muita AIP-käytäntöjä koskevia hyödyllisiä resursseja on kohdassa:</span><span class="sxs-lookup"><span data-stu-id="62978-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="62978-112">Opetusohjelma: Azure Information Protection -käytäntöasetusten määrittäminen ja uuden tarran luominen</span><span class="sxs-lookup"><span data-stu-id="62978-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="62978-113">Azure-tietojen suojauskäytännön määrittäminen</span><span class="sxs-lookup"><span data-stu-id="62978-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="62978-114">Herkkyystarrojen ja niiden käytäntöjen luominen ja määrittäminen</span><span class="sxs-lookup"><span data-stu-id="62978-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="62978-115">Azure Information Protection -suojausta käyttävien yleisten skenaarioiden toimintaohjeet</span><span class="sxs-lookup"><span data-stu-id="62978-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="62978-116">Azure Information Protection -dokumentaation tarkasteleminen</span><span class="sxs-lookup"><span data-stu-id="62978-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="62978-117">Azure-tietojen suojausta koskevat vaatimukset</span><span class="sxs-lookup"><span data-stu-id="62978-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="62978-118">Azure Information Protectionin pika-aloitusopas</span><span class="sxs-lookup"><span data-stu-id="62978-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="62978-119">Lataa Azure Information Protection -asiakasohjelma</span><span class="sxs-lookup"><span data-stu-id="62978-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)