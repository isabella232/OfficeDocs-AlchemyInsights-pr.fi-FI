---
title: Siirtyminen AIP:stä MIP:ksi tai yhdistetyksi osoitetarrojen siirroksi yhteensopivuuskeskuksessa
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
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825368"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="15109-102">Siirtyminen AIP:stä MIP:ksi tai yhdistetyksi osoitetarrojen siirroksi yhteensopivuuskeskuksessa</span><span class="sxs-lookup"><span data-stu-id="15109-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="15109-103">Jos haluat siirtyä AIP-selitteet yhdistettyyn osoitetarraan tietoturva- ja yhteensopivuuskeskuksessa, tee näin:</span><span class="sxs-lookup"><span data-stu-id="15109-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="15109-104">**Suojauksen aktivoiminen Azure-portaalista**</span><span class="sxs-lookup"><span data-stu-id="15109-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="15109-105">Jos et ole vielä tehnyt niin, avaa uusi selainikkuna ja kirjaudu [sisään Azure-portaaliin.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="15109-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="15109-106">Siirry **Azure Information Protection -teriin.**</span><span class="sxs-lookup"><span data-stu-id="15109-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="15109-107">Valitse esimerkiksi keskusvalikossa Kaikki palvelut **ja ala** kirjoittaa Tiedot Suodatin-ruutuun. </span><span class="sxs-lookup"><span data-stu-id="15109-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="15109-108">Valitse **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="15109-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="15109-109">Jos et ole ennen käynyt Azure Information Protection -osaa, [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) katso ohjeet tämän terien lisäämiseksi portaaliin kertakäyttöisillä lisävaiheilla.</span><span class="sxs-lookup"><span data-stu-id="15109-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="15109-110">Jotta voit avata Azure Information Protection -laikan, sinulla on oltava [joko Azure Information Protection Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) -palvelupaketti tai Office 365 -palvelupaketti, joka sisältää oikeuksien hallinnan.</span><span class="sxs-lookup"><span data-stu-id="15109-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="15109-111">Jos sinulla on jokin näistä tilauksia, mutta näet viestin, jonka mukaan kelvollista tilausta ei löydy, ota yhteyttä [Microsoft-tukeen](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) tai käytä vakiotukikanaviasi.</span><span class="sxs-lookup"><span data-stu-id="15109-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="15109-112">Etsi **Hallinta-valikkovaihtoehdot** ja valitse **Suojausaktivointi**.</span><span class="sxs-lookup"><span data-stu-id="15109-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="15109-113">Valitse **Aktivoi** ja vahvista sitten toiminto.</span><span class="sxs-lookup"><span data-stu-id="15109-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="15109-114">Kun aktivointi on valmis, tietopalkissa näkyy teksti Aktivointi **suoritettu.**</span><span class="sxs-lookup"><span data-stu-id="15109-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="15109-115">**Azure Information Protection -tunnisteiden siirtäminen Office 365:n & yhteensopivuuskeskukseen**</span><span class="sxs-lookup"><span data-stu-id="15109-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="15109-116">Varmista, että olet kirjautunut sisään käyttäjänä yleisenä järjestelmänvalvojana.</span><span class="sxs-lookup"><span data-stu-id="15109-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="15109-117">Siirry **Azure Information Protection -teriin.**</span><span class="sxs-lookup"><span data-stu-id="15109-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="15109-118">Valitse **Hallinta-valikkovaihtoehdosta** **Yhdistetty selite**.</span><span class="sxs-lookup"><span data-stu-id="15109-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="15109-119">Valitse **Azure Information Protection - Unified Labeling -laitteessa** **Aktivoi** ja noudata online-ohjeita.</span><span class="sxs-lookup"><span data-stu-id="15109-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="15109-120">**Huomautus:** Varmista, että sinulla on tarvittavat käyttöoikeudet ennen tietoturvakeskuksen & aktivoimista.</span><span class="sxs-lookup"><span data-stu-id="15109-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="15109-121">Lisätietoja on näissä artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="15109-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="15109-122">Onko sinun oltava yleinen järjestelmänvalvoja Azure Information Protectionin määrittämiseksi vai voinko delegoida sen muille järjestelmänvalvojille?</span><span class="sxs-lookup"><span data-stu-id="15109-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="15109-123">Tärkeitä tietoja järjestelmänvalvojan rooleista tietoturva- ja & jälkeen.</span><span class="sxs-lookup"><span data-stu-id="15109-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="15109-124">Lisätietoja AIP:n yhdistetyn osoitetarrojen siirrosta tietoturva- ja yhteensopivuuskeskukseen on kohdassa [Osoitetarrojen siirtäminen.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)</span><span class="sxs-lookup"><span data-stu-id="15109-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
