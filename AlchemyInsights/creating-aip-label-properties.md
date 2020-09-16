---
title: AIP-tarra käytäntöjen luominen
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732172"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="e0824-102">AIP-tarra käytäntöjen luominen</span><span class="sxs-lookup"><span data-stu-id="e0824-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="e0824-103">Azure Information Protectionin (AIP) otsikoita voidaan käyttää kaikkien niiden tietojen kanssa, jotka organisaatio tyypillisesti luo ja tallentaa, henkilö tietojen alimmasta luokituksesta erittäin luottamuksellisten tietojen korkeimpaan luokitukseen.</span><span class="sxs-lookup"><span data-stu-id="e0824-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="e0824-104">Azure Information Protectionin suojaus käytännöt koskevat Azure Information Protectionin (AIP) Classic-asiakas ohjelmaa eikä  [AIP Unified-merkintä asiakasta](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="e0824-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="e0824-105">Voit määrittää useita asioita AIP-käytännössä, kuten esimerkiksi seuraavat vaihto ehdot:</span><span class="sxs-lookup"><span data-stu-id="e0824-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="e0824-106">Vaihto ehto, jonka avulla järjestelmänvalvojat tai käyttäjä voi luokitella ja suojata (valinnaisia) asia kirjoja ja Sähkö posti viestejä</span><span class="sxs-lookup"><span data-stu-id="e0824-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="e0824-107">Asetukset, joilla voit pakottaa luokittelun, kun käyttäjät tallentavat asia kirjoja ja lähettävät sähkö postia</span><span class="sxs-lookup"><span data-stu-id="e0824-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="e0824-108">Asetus, joka lisää Sähkö posti viestin automaattisesti sen liitteiden perusteella.</span><span class="sxs-lookup"><span data-stu-id="e0824-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="e0824-109">Vaihto ehto, joka määrittää, näytetäänkö tieto turva palkki Office-sovelluksissa</span><span class="sxs-lookup"><span data-stu-id="e0824-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="e0824-110">Lisä tietoja Azuren tietojen suojaus käytännöistä on kohdassa [Yleiskatsaus Azure Information Protectionin tieto turva käytäntöön](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="e0824-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="e0824-111">Muita AIP-käytäntöjä koskevia hyödyllisiä resursseja on osoitteessa:</span><span class="sxs-lookup"><span data-stu-id="e0824-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="e0824-112">Opetus ohjelma: Azure-tieto turva käytäntöjen asetusten määrittäminen ja uuden tarran luominen</span><span class="sxs-lookup"><span data-stu-id="e0824-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="e0824-113">Azure-tieto turva käytäntöjen määrittäminen</span><span class="sxs-lookup"><span data-stu-id="e0824-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="e0824-114">Luottamuksellisuusmerkkien ja niiden käytäntöjen luominen ja määrittäminen</span><span class="sxs-lookup"><span data-stu-id="e0824-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="e0824-115">Käyttö oppaat yleisille skenaarioille, jotka käyttävät Azure-tieto suojausta</span><span class="sxs-lookup"><span data-stu-id="e0824-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="e0824-116">Azure Information Protectionin ohjeiden tarkasteleminen</span><span class="sxs-lookup"><span data-stu-id="e0824-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="e0824-117">Azure Information Protectionin vaatimukset</span><span class="sxs-lookup"><span data-stu-id="e0824-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="e0824-118">Azure Information Protectionin Pika-aloitus opas</span><span class="sxs-lookup"><span data-stu-id="e0824-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="e0824-119">Lataa Azure Information Protectionin asiakas</span><span class="sxs-lookup"><span data-stu-id="e0824-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)