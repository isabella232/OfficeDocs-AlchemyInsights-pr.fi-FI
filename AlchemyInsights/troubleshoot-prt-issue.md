---
title: PRT-ongelman vian määritys
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573495"
---
# <a name="troubleshoot-prt-issue"></a><span data-ttu-id="562a4-102">PRT-ongelman vian määritys</span><span class="sxs-lookup"><span data-stu-id="562a4-102">Troubleshoot PRT issue</span></span>

<span data-ttu-id="562a4-103">Jotta kaikki laitteet saataisiin todennettua, niiden on oltava täysin rekisteröity ja hyvässä kunnossa ja niiden on pystyttävä hankkimaan ensisijaiset päivitys tunnus (PRT).</span><span class="sxs-lookup"><span data-stu-id="562a4-103">For any device to complete getting authenticated, it must be fully registered and in good state and able to acquire a Primary Refresh Token (PRT).</span></span>

<span data-ttu-id="562a4-104">Hybridi Azure AD Join-rekisteröinti prosessi edellyttää, että laitteet ovat yrityksen verkossa.</span><span class="sxs-lookup"><span data-stu-id="562a4-104">The hybrid Azure AD join registration process requires devices to be on a corporate network.</span></span> <span data-ttu-id="562a4-105">Se toimii myös VPN-yhteyden kautta, mutta siihen liittyy joitakin varoituksista.</span><span class="sxs-lookup"><span data-stu-id="562a4-105">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="562a4-106">Olemme kuulleet, että asiakkaat tarvitsevat apua vian määrityksessä hybridi Azure AD Join-rekisteröinti prosessissa etätyöolosuhteissa.</span><span class="sxs-lookup"><span data-stu-id="562a4-106">We’ve heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote-work circumstances.</span></span> <span data-ttu-id="562a4-107">Seuraavassa on tietoja siitä, mitä kone pellin alle tapahtuu rekisteröinti prosessin aikana.</span><span class="sxs-lookup"><span data-stu-id="562a4-107">Here’s a breakdown of what’s happening ‘under the hood’ during the registration process.</span></span>

<span data-ttu-id="562a4-108">**Pilvi todennus ympäristö (Azure AD Password hash-synkronoinnin tai läpi vienti todennuksen avulla)**</span><span class="sxs-lookup"><span data-stu-id="562a4-108">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="562a4-109">Tätä rekisteröinti kulkua kutsutaan myös nimellä "synkronointi liitos".</span><span class="sxs-lookup"><span data-stu-id="562a4-109">This registration flow is also known as “Sync Join”.</span></span>

1. <span data-ttu-id="562a4-110">Windows 10 havaitsee SCP-tietueen, kun käyttäjä kirjautuu laitteeseen.</span><span class="sxs-lookup"><span data-stu-id="562a4-110">Windows 10 discovers an SCP record upon user logging on to the device.</span></span>
    1. <span data-ttu-id="562a4-111">Laite yrittää ensin hakea vuokra ajan tietoja asiakas puolen SCP-rekisteristä [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="562a4-111">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="562a4-112">Katso lisä tietoja tästä [asia kirjasta](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="562a4-112">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    2. <span data-ttu-id="562a4-113">Jos se epäonnistuu, laite kommunikoi paikallisen Active Directoryn (AD) kanssa saadakseen vuokra ajan tietoja palvelun yhteys pisteestä (SCP).</span><span class="sxs-lookup"><span data-stu-id="562a4-113">If it fails, the device communicates with on-premises Active Directory (AD) to get tenant information from Service Connection Point (SCP).</span></span> <span data-ttu-id="562a4-114">Jos haluat tarkistaa SCP-toiminnon, Lue tämä [asia kirja](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="562a4-114">To verify SCP, please refer to this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span> 

> [!NOTE]
> <span data-ttu-id="562a4-115">Suosittelemme, että SCP otetaan käyttöön MAINOKSESSA ja että se on käytössä vain asiakas puolen SCP: ssa alkuperäisen kelpoisuuden tarkistamista varten.</span><span class="sxs-lookup"><span data-stu-id="562a4-115">We recommend enabling SCP in the AD and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="562a4-116">Windows 10 yrittää muodostaa yhteyden Azure AD:hen järjestelmä kontekstissa ja todentaa itsensä Azure AD:hen.</span><span class="sxs-lookup"><span data-stu-id="562a4-116">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span> <span data-ttu-id="562a4-117">Voit tarkistaa, Voiko laite käyttää Microsoft-resursseja järjestelmä tilillä, käyttämällä testi laitteen rekisteröinnin yhteys komento sarjaa.</span><span class="sxs-lookup"><span data-stu-id="562a4-117">You can verify if the device can access Microsoft resources under the system account by using the Test Device Registration Connectivity script.</span></span>

3. <span data-ttu-id="562a4-118">Windows 10 luo itse allekirjoitetun varmenteen ja tallentaa sen paikallisessa MAINOKSESSA tieto kone-objektiin.</span><span class="sxs-lookup"><span data-stu-id="562a4-118">Windows 10 generates a self-signed certificate and stores it under the computer object in on-premises AD.</span></span> <span data-ttu-id="562a4-119">Tämä edellyttää näkö yhteys toimi alueen ohjaus koneeseen.</span><span class="sxs-lookup"><span data-stu-id="562a4-119">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="562a4-120">Laite objekti, joka sisältää varmenteen, synkronoidaan Azure AD:hen Azure AD Connectin kautta.</span><span class="sxs-lookup"><span data-stu-id="562a4-120">A device object that has a certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="562a4-121">Synkronointi sykli on oletusarvoisesti 30 minuutin välein, mutta se määräytyy Azure AD Connectin määritysten mukaan.</span><span class="sxs-lookup"><span data-stu-id="562a4-121">Sync cycle is every 30 minutes by default, but it depends on configuration of Azure AD Connect.</span></span> <span data-ttu-id="562a4-122">Katso lisä tietoja tästä [asia kirjasta](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="562a4-122">For more information, please refer to this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="562a4-123">Tässä vaiheessa sinun pitäisi pystyä näkemään aihe laite "odottaa"-tilassa, joka on Azure-portaalin Device Blade-kohdassa.</span><span class="sxs-lookup"><span data-stu-id="562a4-123">At this stage, you should be able to see the subject device in “Pending” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="562a4-124">Kun seuraava käyttäjä on kirjautunut Windows 10: een, rekisteröinti valmistuu.</span><span class="sxs-lookup"><span data-stu-id="562a4-124">At the next user login to Windows 10, the registration will be completed.</span></span> 

> [!NOTE]
> <span data-ttu-id="562a4-125">Jos käytät VPN-yhteyttä ja kirjautuminen ulos-Kirjautumisprosessi lopettaa toimi alue yhteyden, voit käynnistää rekisteröinnin manuaalisesti:</span><span class="sxs-lookup"><span data-stu-id="562a4-125">If you're on VPN and a logoff-login process terminates the domain connectivity, you can trigger registration manually:</span></span>
 1. <span data-ttu-id="562a4-126">Ongelma dsregcmd/Join paikallisesti järjestelmänvalvojan kehotteesta tai etäyhteyden kautta PSExec tieto koneeseen.</span><span class="sxs-lookup"><span data-stu-id="562a4-126">Issue a dsregcmd /join locally on admin prompt or remotely via PSExec to your PC.</span></span> <span data-ttu-id="562a4-127">Esimerkiksi PsExec-n \\ win10client01 cmd, dsregcmd/Join</span><span class="sxs-lookup"><span data-stu-id="562a4-127">For example, PsExec -s \\win10client01 cmd, dsregcmd /join</span></span>

 2. <span data-ttu-id="562a4-128">Lisä tietoja yhdistelmä liitoksen ongelmista on kohdassa laitteet- [ongelman vian määritys](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span><span class="sxs-lookup"><span data-stu-id="562a4-128">For more details on Hybrid Join issues, see [Troubleshoot devices Issue](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).</span></span>
