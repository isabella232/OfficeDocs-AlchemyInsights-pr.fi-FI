---
title: Laite odottaa-tilassa
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/11/2020
ms.locfileid: "49678480"
---
# <a name="device-in-pending-state"></a><span data-ttu-id="0fcec-102">Laite odottaa-tilassa</span><span class="sxs-lookup"><span data-stu-id="0fcec-102">Device in pending state</span></span>

<span data-ttu-id="0fcec-103">**Edellytykset**</span><span class="sxs-lookup"><span data-stu-id="0fcec-103">**Prerequisites:**</span></span>

1. <span data-ttu-id="0fcec-104">Jos olet määrittämässä laitteiden rekisteröintejä ensimmäistä kertaa, varmista, että olet tarkistanut [laitteen hallinnan käytön Azure Active Directoryssa (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) , joka ohjaa sinua käyttämään laitteita Azure AD:n hallinnassa.</span><span class="sxs-lookup"><span data-stu-id="0fcec-104">If you are setting up device registrations for the first time, please ensure that you have reviewed [Introduction to device management in Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) that will guide you on how to get devices under the control of Azure AD.</span></span>
2. <span data-ttu-id="0fcec-105">Jos olet rekisteröimässä laitteita Azure AD:hen suoraan ja rekisteröimällä ne Intuneen, sinun on varmistettava, että olet [määrittänyt Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) ja että [käyttö oikeus](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) on ensin käytössä.</span><span class="sxs-lookup"><span data-stu-id="0fcec-105">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
3. <span data-ttu-id="0fcec-106">Varmista, että sinulla on oikeus suorittaa toimintoja Azure AD:ssä ja paikallisessa MAINOKSESSA.</span><span class="sxs-lookup"><span data-stu-id="0fcec-106">Ensure you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="0fcec-107">Vain Azure AD:ssä oleva yleinen hallinnoija voi hallita laite rekisteröintien asetuksia.</span><span class="sxs-lookup"><span data-stu-id="0fcec-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="0fcec-108">Lisäksi jos määrität automaattisia rekisteröintejä paikallisessa Active Directoryssa, sinun on oltava Active Directoryn ja AD FS:N järjestelmänvalvoja (tarvittaessa).</span><span class="sxs-lookup"><span data-stu-id="0fcec-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="0fcec-109">Hybridi Azure AD Join-rekisteröinti prosessi edellyttää, että laitteet ovat yrityksen verkossa.</span><span class="sxs-lookup"><span data-stu-id="0fcec-109">The hybrid Azure AD join registration process requires devices to be on corporate network.</span></span> <span data-ttu-id="0fcec-110">Se toimii myös VPN-yhteyden kautta, mutta siihen liittyy joitakin varoituksista.</span><span class="sxs-lookup"><span data-stu-id="0fcec-110">It also works over VPN but there are some caveats to that.</span></span> <span data-ttu-id="0fcec-111">Olemme kuulleet, että asiakkaat tarvitsevat apua vian määrityksessä hybridi Azure AD Join-rekisteröinti prosessissa etätyöolosuhteissa.</span><span class="sxs-lookup"><span data-stu-id="0fcec-111">We have heard customers needing assistance with troubleshooting the hybrid Azure AD join registration process under remote work circumstances.</span></span>

<span data-ttu-id="0fcec-112">**Pilvi todennus ympäristö (Azure AD Password hash-synkronoinnin tai läpi vienti todennuksen avulla)**</span><span class="sxs-lookup"><span data-stu-id="0fcec-112">**Cloud authentication environment (using Azure AD password hash sync or pass-through authentication)**</span></span>

<span data-ttu-id="0fcec-113">Tätä rekisteröinti kulkua kutsutaan myös nimellä "synkronointi liitos".</span><span class="sxs-lookup"><span data-stu-id="0fcec-113">This registration flow is also known as “Sync Join”.</span></span>

<span data-ttu-id="0fcec-114">Tässä on erittely siitä, mitä rekisteröinti prosessin aikana tapahtuu:</span><span class="sxs-lookup"><span data-stu-id="0fcec-114">Here is a breakdown of what happens during the registration process:</span></span>

1. <span data-ttu-id="0fcec-115">Windows 10 havaitsee palvelun yhteys pisteen (SCP) tietueen, kun käyttäjä kirjautuu laitteeseen.</span><span class="sxs-lookup"><span data-stu-id="0fcec-115">Windows 10 discovers Service Connection Point (SCP) record when the user logs on to the device.</span></span>

    1. <span data-ttu-id="0fcec-116">Laite yrittää ensin hakea vuokra ajan tietoja asiakas puolen SCP-rekisteristä [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span><span class="sxs-lookup"><span data-stu-id="0fcec-116">The device first tries to retrieve tenant information from client-side SCP in registry [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD].</span></span> <span data-ttu-id="0fcec-117">Lisä tietoja on kohdassa [asia kirja](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span><span class="sxs-lookup"><span data-stu-id="0fcec-117">For more information, see [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).</span></span>
    1. <span data-ttu-id="0fcec-118">Jos se epäonnistuu, laite kommunikoi paikallisen Active Directoryn kanssa ja saa vuokra ajan tietoja SCP-tieto kannasta.</span><span class="sxs-lookup"><span data-stu-id="0fcec-118">If it fails, the device communicates with on-premises Active Directory to get tenant information from SCP.</span></span> <span data-ttu-id="0fcec-119">Jos haluat tarkistaa SCP-tiedoston, Lue tämä [asia kirja](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span><span class="sxs-lookup"><span data-stu-id="0fcec-119">To verify SCP, refer this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).</span></span>

    > [!NOTE]
    > <span data-ttu-id="0fcec-120">Suosittelemme, että SCP otetaan käyttöön Active Directoryssa ja että se on käytössä vain asiakas puolen SCP: ssa alkuperäistä vahvistusta varten.</span><span class="sxs-lookup"><span data-stu-id="0fcec-120">We recommend enabling SCP in the Active Directory and only using client-side SCP for initial validation.</span></span>

2. <span data-ttu-id="0fcec-121">Windows 10 yrittää muodostaa yhteyden Azure AD:hen järjestelmä kontekstissa ja todentaa itsensä Azure AD:hen.</span><span class="sxs-lookup"><span data-stu-id="0fcec-121">Windows 10 tries to communicate with Azure AD under the system context to authenticate itself against Azure AD.</span></span>

    <span data-ttu-id="0fcec-122">Voit tarkistaa, Voiko laite käyttää Microsoft-resursseja järjestelmä tilillä, käyttämällä [testi laitteen rekisteröinnin yhteys komento sarjaa](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span><span class="sxs-lookup"><span data-stu-id="0fcec-122">You can verify if the device can access Microsoft resources under the system account by using the [Test Device Registration Connectivity script](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).</span></span>

3. <span data-ttu-id="0fcec-123">Windows 10 luo itse allekirjoitetun varmenteen ja tallentaa sen paikallisen Active Directoryn tieto kone-objektiin.</span><span class="sxs-lookup"><span data-stu-id="0fcec-123">Windows 10 generates self-signed certificate and stores it under the computer object in on-premises Active Directory.</span></span> <span data-ttu-id="0fcec-124">Tämä edellyttää näkö yhteys toimi alueen ohjaus koneeseen.</span><span class="sxs-lookup"><span data-stu-id="0fcec-124">This requires line-of-sight to Domain Controller.</span></span>

4. <span data-ttu-id="0fcec-125">Laite objekti, jonka varmenne on synkronoitu Azure AD:hen Azure AD Connectin kautta.</span><span class="sxs-lookup"><span data-stu-id="0fcec-125">Device object that has certificate gets synchronized to Azure AD via Azure AD Connect.</span></span> <span data-ttu-id="0fcec-126">Synkronointi sykli on oletusarvoisesti 30 minuutin välein, mutta se määräytyy Azure AD Connectin määritysten mukaan.</span><span class="sxs-lookup"><span data-stu-id="0fcec-126">Sync cycle is every 30 minutes by default, but it depends on the configuration of Azure AD Connect.</span></span> <span data-ttu-id="0fcec-127">Jos haluat lisä tietoja, Lue tämä [asia kirja](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span><span class="sxs-lookup"><span data-stu-id="0fcec-127">For more information, refer this [document](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).</span></span>

5. <span data-ttu-id="0fcec-128">Tässä vaiheessa sinun pitäisi pystyä näkemään aihe laite "**odottaa**"-tilassa, joka on Azure-portaalin Device Blade-kohdassa.</span><span class="sxs-lookup"><span data-stu-id="0fcec-128">At this stage, you should be able to see the subject device in “**Pending**” state under Device blade of Azure Portal.</span></span>

6. <span data-ttu-id="0fcec-129">Kun seuraava käyttäjä on kirjautunut Windows 10: een, rekisteröinti valmistuu.</span><span class="sxs-lookup"><span data-stu-id="0fcec-129">At the next user login to Windows 10, the registration will be completed.</span></span>

    > [!NOTE]
    > <span data-ttu-id="0fcec-130">Jos käytät VPN-yhteyttä ja uloskirjautuminen/Kirjautuminen lopettaa toimi alueen yhdistämisen, voit laukaista rekisteröinnin manuaalisesti.</span><span class="sxs-lookup"><span data-stu-id="0fcec-130">If you are on VPN and logoff/login terminates the domain connectivity, you can trigger registration manually.</span></span> <span data-ttu-id="0fcec-131">Voit tehdä sen seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="0fcec-131">To do that:</span></span>
    >
    > <span data-ttu-id="0fcec-132">Ongelma `dsregcmd /join` paikallisesti järjestelmänvalvojan kehotteessa tai etäyhteyden kautta PSExec tieto koneeseen.</span><span class="sxs-lookup"><span data-stu-id="0fcec-132">Issue a `dsregcmd /join` locally on admin prompt or remotely via PSExec to your PC.</span></span>
    >
    > <span data-ttu-id="0fcec-133">Esimerkki: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span><span class="sxs-lookup"><span data-stu-id="0fcec-133">For example: `PsExec -s \\win10client01 cmd, dsregcmd /join`</span></span>

<span data-ttu-id="0fcec-134">Yleisiä ongelmia Azure Active Directory-laitteen rekisteröinnissä on kohdassa [laitteiden usein kysytyt kysymykset](https://docs.microsoft.com/azure/active-directory/devices/faq).</span><span class="sxs-lookup"><span data-stu-id="0fcec-134">For common issues with Azure Active Directory device registration, see [Devices FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq).</span></span>
