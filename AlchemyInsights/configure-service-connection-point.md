---
title: Palveluyhteyspisteen (SCP) määrittäminen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035452"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="730fb-102">Palvelun yhteyspisteen (SCP) määrittäminen</span><span class="sxs-lookup"><span data-stu-id="730fb-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="730fb-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="730fb-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="730fb-104">**Syy:** SCP-objektin lukeminen ja Azure AD -vuokraajan tietojen saaminen ei onnistu</span><span class="sxs-lookup"><span data-stu-id="730fb-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="730fb-105">**Ratkaisu:** Katso kohta [Palveluyhteyspisteen määrittäminen](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="730fb-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="730fb-106">**Toimintasuunnitelma**</span><span class="sxs-lookup"><span data-stu-id="730fb-106">**Action plan**</span></span>

- <span data-ttu-id="730fb-107">Tarkista, onko laite saanut GPO:n hallittua vahvistusta varten.</span><span class="sxs-lookup"><span data-stu-id="730fb-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="730fb-108">Varmista, että GPO on luonut rekisteriavaimet.</span><span class="sxs-lookup"><span data-stu-id="730fb-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="730fb-109">Varmista, että sinulla on kaksi avainta, jotka on luotu hakemistotunnuksella ja onmicrosoft-toimialueella.</span><span class="sxs-lookup"><span data-stu-id="730fb-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="730fb-110">**Asiakaspuolen rekisteriasetuksen määrittäminen SCP:lle**</span><span class="sxs-lookup"><span data-stu-id="730fb-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="730fb-111">Seuraavan esimerkin avulla voit luoda ryhmäkäytäntöobjektin ottaaksesi käyttöön rekisteriasetuksen, joka määrittää SCP-merkinnän laitteiden rekisterissä.</span><span class="sxs-lookup"><span data-stu-id="730fb-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="730fb-112">Avaa ryhmäkäytäntöjen hallintakonsoli ja luo uusi ryhmäkäytäntöobjekti toimialueellesi.</span><span class="sxs-lookup"><span data-stu-id="730fb-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="730fb-113">Anna juuri luomallesi GPO:lle nimi (esimerkiksi ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="730fb-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="730fb-114">Muokkaa käyttäjäkäytäntöobjektia ja etsi seuraava polku: tietokoneen > asetukset > Windowsin > **rekisteriin.**</span><span class="sxs-lookup"><span data-stu-id="730fb-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="730fb-115">Napsauta Rekisteri-kohtaa **hiiren kakkospainikkeella** **ja valitse > rekisterikohde.**</span><span class="sxs-lookup"><span data-stu-id="730fb-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="730fb-116">Määritä **Yleiset-välilehdessä** seuraavat asetukset:</span><span class="sxs-lookup"><span data-stu-id="730fb-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="730fb-117">**Toiminto:** Päivitä</span><span class="sxs-lookup"><span data-stu-id="730fb-117">**Action**: Update</span></span>
    
- <span data-ttu-id="730fb-118">**Rakenne :** HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="730fb-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="730fb-119">**Avainpolku:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="730fb-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="730fb-120">**Arvon nimi**: Vuokraajatunnus</span><span class="sxs-lookup"><span data-stu-id="730fb-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="730fb-121">**Arvotyyppi:** REG_SZ</span><span class="sxs-lookup"><span data-stu-id="730fb-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="730fb-122">**Arvotiedot:** Azure AD -esiintymän GUID- tai hakemistotunnus (tämä arvo > **Azure Active Directory ->-ominaisuuksien > hakemistotunnuksesta)**</span><span class="sxs-lookup"><span data-stu-id="730fb-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="730fb-123">Valitse **OK**.</span><span class="sxs-lookup"><span data-stu-id="730fb-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="730fb-124">Napsauta Rekisteri-kohtaa **hiiren kakkospainikkeella** **ja valitse > rekisterikohde.**</span><span class="sxs-lookup"><span data-stu-id="730fb-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="730fb-125">Määritä **Yleiset-välilehdessä** seuraavat asetukset:</span><span class="sxs-lookup"><span data-stu-id="730fb-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="730fb-126">**Toiminto:** Päivitä</span><span class="sxs-lookup"><span data-stu-id="730fb-126">**Action**: Update</span></span>
    
- <span data-ttu-id="730fb-127">**Rakenne :** HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="730fb-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="730fb-128">**Avainpolku:** SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="730fb-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="730fb-129">**Arvon nimi**: VuokraajanNimi</span><span class="sxs-lookup"><span data-stu-id="730fb-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="730fb-130">**Arvotyyppi:** REG_SZ</span><span class="sxs-lookup"><span data-stu-id="730fb-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="730fb-131">**Arvon tiedot:** Varmennettu toimialuenimesi, jos käytät liitettyä ympäristöä, kuten AD FS:ää.</span><span class="sxs-lookup"><span data-stu-id="730fb-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="730fb-132">Varmennettu toimialuenimi tai onmicrosoft.com toimialuenimi (esimerkiksi contoso.onmicrosoft).com, jos käytät hallittua ympäristöä</span><span class="sxs-lookup"><span data-stu-id="730fb-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="730fb-133">Valitse **OK**.</span><span class="sxs-lookup"><span data-stu-id="730fb-133">Click **OK**.</span></span>

7. <span data-ttu-id="730fb-134">Sulje juuri luodun GPO:n editori.</span><span class="sxs-lookup"><span data-stu-id="730fb-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="730fb-135">Linkitä juuri luotu GPO haluttuun OU:han, joka sisältää toimialueeseen liitettyja tietokoneita, jotka kuuluvat valvotulle koontipopulaatiolle.</span><span class="sxs-lookup"><span data-stu-id="730fb-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="730fb-136">Lisätietoja on kohdassa [Azure AD -yhdistelmäympäristön liitoksen hallittu vahvistus – Azure AD | Microsoft Docs ja](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) [Azure Active Directoryyn liitettyjen yhdistelmälaitteiden | Microsoft Docs.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current)</span><span class="sxs-lookup"><span data-stu-id="730fb-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









