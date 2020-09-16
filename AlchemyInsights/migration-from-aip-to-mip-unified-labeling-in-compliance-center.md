---
title: Siirtyminen AIP-ohjelmassa VÄHIMMÄISTUONTIHINNAN/yhdistetyn merkinnän kanssa yhteensopivuus keskuksessa
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
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674323"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="9c07f-102">Siirtyminen AIP-ohjelmassa VÄHIMMÄISTUONTIHINNAN/yhdistetyn merkinnän kanssa yhteensopivuus keskuksessa</span><span class="sxs-lookup"><span data-stu-id="9c07f-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="9c07f-103">Jos haluat siirtyä AIP-otsikoista tieto turva-ja yhteensopivuus keskuksen yhdenmukaisiin merkintä toimiin, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="9c07f-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="9c07f-104">**Ota suojaus käyttöön Azure-portaalissa**</span><span class="sxs-lookup"><span data-stu-id="9c07f-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="9c07f-105">Jos et ole vielä tehnyt niin, avaa uusi selain ikkuna ja [Kirjaudu sisään Azure-portaaliin](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="9c07f-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="9c07f-106">Siirry **Azure Information Protectionin** terään.</span><span class="sxs-lookup"><span data-stu-id="9c07f-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="9c07f-107">Valitse esimerkiksi keskitin-valikossa **Kaikki palvelut** ja ala kirjoittaa **tietoja** suodatin-ruutuun.</span><span class="sxs-lookup"><span data-stu-id="9c07f-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="9c07f-108">Valitse **Azure Information Protectionin**.</span><span class="sxs-lookup"><span data-stu-id="9c07f-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="9c07f-109">Jos et ole aiemmin käyttänyt Azure Information Protectionin terää, katso [lisä ohjeita](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) tämän lavan lisäämiseen portaaliin.</span><span class="sxs-lookup"><span data-stu-id="9c07f-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="9c07f-110">Jos haluat avata Azure Information Protectionin terän, sinulla on oltava joko [Azure Information Protectionin Premium](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) -palvelu paketin tai Office 365-palvelu paketin, joka sisältää oikeuksien hallinnan.</span><span class="sxs-lookup"><span data-stu-id="9c07f-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="9c07f-111">Jos sinulla on jokin näistä paketeista, mutta saat ilmoituksen siitä, että kelvollista tilausta ei löydy, [Ota yhteyttä Microsoftin tukeen](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) tai käytä tavallisia tuki kanavia.</span><span class="sxs-lookup"><span data-stu-id="9c07f-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="9c07f-112">Etsi **Hallitse** -valikon vaihto ehdot ja valitse **Suojaus aktivointi**.</span><span class="sxs-lookup"><span data-stu-id="9c07f-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="9c07f-113">Valitse **Aktivoi**ja vahvista sitten toiminto.</span><span class="sxs-lookup"><span data-stu-id="9c07f-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="9c07f-114">Kun Akti vointi on valmis, tieto palkissa näkyy **Akti voinnin onnistuminen**.</span><span class="sxs-lookup"><span data-stu-id="9c07f-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="9c07f-115">**Azure-tieto turva merkintöjen siirtäminen Office 365-suojaus & yhteensopivuus keskukseen**</span><span class="sxs-lookup"><span data-stu-id="9c07f-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="9c07f-116">Varmista, että olet kirjautunut sisään käyttäjänä, jolla on yleinen hallinta oikeus.</span><span class="sxs-lookup"><span data-stu-id="9c07f-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="9c07f-117">Siirry **Azure Information Protectionin** terään.</span><span class="sxs-lookup"><span data-stu-id="9c07f-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="9c07f-118">Valitse **hallinta** -valikko-vaihto ehdossa **yhdistetty merkintä**.</span><span class="sxs-lookup"><span data-stu-id="9c07f-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="9c07f-119">Valitse **Azure Information Protectionin yhdistetyn** merkinnän Blade-kohdassa **Aktivoi** ja noudata online-ohjeita.</span><span class="sxs-lookup"><span data-stu-id="9c07f-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="9c07f-120">**Huomautus**: Varmista, että sinulla on tarvittavat käyttö oikeudet, ennen kuin Akti voit suojaus & yhteensopivuus keskuksen siirron.</span><span class="sxs-lookup"><span data-stu-id="9c07f-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="9c07f-121">Lisä tietoja on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="9c07f-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="9c07f-122">Onko sinun oltava yleinen järjestelmänvalvoja, jotta voit määrittää Azure Information Protectionin tai delegoida sen muille järjestelmänvalvojille?</span><span class="sxs-lookup"><span data-stu-id="9c07f-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="9c07f-123">Tärkeitä tietoja järjestelmänvalvojan rooleista tieto turvaan & yhteensopivuus keskukseen siirryttäessä.</span><span class="sxs-lookup"><span data-stu-id="9c07f-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="9c07f-124">Lisä tietoja AIP:tä yhdistetystä merkintöjen siirtämisestä tieto turva-ja yhteensopivuus keskukseen on kohdassa [tunnisteiden siirtäminen](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="9c07f-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
