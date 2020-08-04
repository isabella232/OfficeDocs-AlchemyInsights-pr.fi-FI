---
title: Asiakkaan todennusvarmenteen käyttöönoton vianmääritys
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555001"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="dd33a-102">Asiakkaan todennusvarmenteen käyttöönoton vianmääritys</span><span class="sxs-lookup"><span data-stu-id="dd33a-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="dd33a-103">Intune NDES/SCEP- ja PKCS/PFX-asiakassertifikaattiprofiileja käytetään yleisesti yhdessä muiden profiilityyppien, kuten Wifin, VPN:n ja sähköpostin, kanssa, jotta käyttäjät voivat todentaa yrityksen resurssit.</span><span class="sxs-lookup"><span data-stu-id="dd33a-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="dd33a-104">Kun nämä profiilityypit on linkitetty asiakassertifikaattiprofiiliin, se riippuu kyseisen profiilin onnistuneesta käyttöönotosta.</span><span class="sxs-lookup"><span data-stu-id="dd33a-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="dd33a-105">Asiakassertifikaattiprofiilin alkuinfrastruktuurin asetukset ja siihen liittyvät määritykset edellyttävät usein vianmääritystä.</span><span class="sxs-lookup"><span data-stu-id="dd33a-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="dd33a-106">Vaiheittaiset ohjeet NDES-liittimen onnistuneeseen asennukseen ja vianmääritysohjeet varmenteiden käyttöönottoon liittyvien ongelmien eristämiseksi ovat seuraavissa ohjeissa:</span><span class="sxs-lookup"><span data-stu-id="dd33a-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="dd33a-107">Määritä infrastruktuuri tukemaan SCEP:tä Intunella</span><span class="sxs-lookup"><span data-stu-id="dd33a-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="dd33a-108">Yleistä SCEP-varmenneprofiilien vianmäärityksestä Microsoft Intunen avulla</span><span class="sxs-lookup"><span data-stu-id="dd33a-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="dd33a-109">Tarkista kokoonpano käyttämällä viitattuja powershell-komentosarjoja.</span><span class="sxs-lookup"><span data-stu-id="dd33a-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="dd33a-110">Lisätietoja on kohdassa [Intune Certificate Connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="dd33a-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="dd33a-111">**Muita yleisiä kysymyksiä**</span><span class="sxs-lookup"><span data-stu-id="dd33a-111">**Other common issues**</span></span>

<span data-ttu-id="dd33a-112">**Kun yritän asentaa Intune-varmenneliittimen NDES-yhdistinpalvelimeen, näyttöön tulee sanoma "Varmennepyynnön salasanaa ei voi vahvistaa. Sitä on ehkä jo käytetty. Hanki uusi salasana, jonka haluat lähettää tämän pyynnön yhteydessä."**</span><span class="sxs-lookup"><span data-stu-id="dd33a-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="dd33a-113">Tämä sanoma tarkoittaa, että sertifikaattiyhdistimen asennus on suoritettava järjestelmänvalvojana.</span><span class="sxs-lookup"><span data-stu-id="dd33a-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="dd33a-114">Joissakin ympäristöissä palvelimissa, joissa Intune-varmenne suoritetaan, on käytettävä välityspalvelinta yhteyden muodostamiseen Intuneen, joten Varmenteen yhdistimen on käytettävä välityspalvelinta.</span><span class="sxs-lookup"><span data-stu-id="dd33a-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="dd33a-115">Joissakin tapauksissa NDES Connector ohittaa määritetyt välityspalvelimen asetukset, ja välityspalvelimen asetukset on ehkä määritettävä paikallisen järjestelmän suojauskontekstissa.</span><span class="sxs-lookup"><span data-stu-id="dd33a-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="dd33a-116">Liuos on jotta ajelu Jäsentenvälinen Tehdä tutkimusmatka koska ELIMISTÖ ja configure valtuutettu edustaja kotona IE.</span><span class="sxs-lookup"><span data-stu-id="dd33a-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="dd33a-117">Kun Intune Connector Service on käynnistetty uudelleen, NDES-liitin muodostaa yhteyden Intuneen.</span><span class="sxs-lookup"><span data-stu-id="dd33a-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="dd33a-118">**Käyttäjälaitteet eivät enää saa SCEP-sertifikaatteja NDES:ltä.**</span><span class="sxs-lookup"><span data-stu-id="dd33a-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="dd33a-119">On mahdollista, että NDES-palvelimelle myönnetty ja NDES-yhdistimen asennuksen aikana määritetty asiakkaan todennusvarmenne on vanhentunut tai puuttuu.</span><span class="sxs-lookup"><span data-stu-id="dd33a-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="dd33a-120">Voit ratkaista ongelman:</span><span class="sxs-lookup"><span data-stu-id="dd33a-120">To resolve:</span></span> 
 
1. <span data-ttu-id="dd33a-121">Poista NDES-liittimen asennus.</span><span class="sxs-lookup"><span data-stu-id="dd33a-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="dd33a-122">Näiden tietojen avulla voit pyytää uutta asiakkaan todennus- tai palvelimen todennusvarmennetta:</span><span class="sxs-lookup"><span data-stu-id="dd33a-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="dd33a-123">Aiheen nimi: CN=external fqdn</span><span class="sxs-lookup"><span data-stu-id="dd33a-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="dd33a-124">Aihe vaihtoehtoinen nimi (molemmat ovat pakollisia): DNS=ulkoinen fqdn, DNS=sisäinen fqdn</span><span class="sxs-lookup"><span data-stu-id="dd33a-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="dd33a-125">Asenna NDES-liitin uudelleen uudella varmenteella.</span><span class="sxs-lookup"><span data-stu-id="dd33a-125">Reinstall the NDES connector with the new certificate.</span></span>