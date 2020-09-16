---
title: Asiakkaan todennus varmenteen käyttöönoton vian määritys
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658983"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="c91fa-102">Asiakkaan todennus varmenteen käyttöönoton vian määritys</span><span class="sxs-lookup"><span data-stu-id="c91fa-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="c91fa-103">Intune NDES/SCEP-ja PKCS/PFX-asiakas sertifikaattien profiileja käytetään yleisesti yhdessä muiden profiilien kanssa, kuten WiFi, VPN ja Sähkö posti, jotta käyttäjät voivat todentaa yrityksen resurssit.</span><span class="sxs-lookup"><span data-stu-id="c91fa-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="c91fa-104">Kun nämä profiili tyypit on linkitetty asiakas sertifikaatti profiiliin, ne määräytyvät kyseisen profiilin onnistuneen käyttöönoton mukaan.</span><span class="sxs-lookup"><span data-stu-id="c91fa-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="c91fa-105">Alkuperäisen infrastruktuurin määrittäminen ja siihen liittyvät asiakas sertifikaatti profiilin määritykset vaativat usein vian määritystä.</span><span class="sxs-lookup"><span data-stu-id="c91fa-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="c91fa-106">Vaiheittaiset ohjeet NDES-yhdistimen onnistuneeseen määrittämiseen ja vian määritys ohjeisiin varmenteen käyttöönottoon liittyvien ongelmien eristämiseksi on kohdassa:</span><span class="sxs-lookup"><span data-stu-id="c91fa-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="c91fa-107">Infrastruktuurin määrittäminen tuke, jos haluat, että SCEP on Intune</span><span class="sxs-lookup"><span data-stu-id="c91fa-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="c91fa-108">Yleistä SP-varmenne profiilien vian määrityksestä Microsoft Intunella</span><span class="sxs-lookup"><span data-stu-id="c91fa-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="c91fa-109">Käytä viitattua PowerShell-komento sarjoja määritysten vahvistamiseen.</span><span class="sxs-lookup"><span data-stu-id="c91fa-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="c91fa-110">Lisä tietoja on kohdassa [Intune-varmenne liittimen tarkistus komento sarjat](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="c91fa-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="c91fa-111">**Muita yleisiä ongelmia**</span><span class="sxs-lookup"><span data-stu-id="c91fa-111">**Other common issues**</span></span>

<span data-ttu-id="c91fa-112">**Kun yritän asentaa Intune-varmenne yhdistimen NDES Connector Server-palvelimeen, näyttöön tulee sanoma "varmenne pyynnön Sala sanaa ei voi vahvistaa. Sitä on ehkä jo käytetty. Hanki uusi sala sana, jotta voit lähettää pyynnön tällä pyynnöllä. "**</span><span class="sxs-lookup"><span data-stu-id="c91fa-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="c91fa-113">Tämä viesti tarkoittaa, että sinun on suoritettava varmenne liittimen asennus järjestelmänvalvojana.</span><span class="sxs-lookup"><span data-stu-id="c91fa-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="c91fa-114">Joissain ympäristöissä palvelinten, joissa Intune-varmenne suoritetaan, tulee käyttää välitys palvelinta yhteyden muodostamiseen Intuneen, joten varmenne yhdistimen on käytettävä välitys palvelinta.</span><span class="sxs-lookup"><span data-stu-id="c91fa-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="c91fa-115">Joissakin tapa uksissa NDES-yhdistin ohittaa määritetyt välitys palvelimen asetukset ja saattaa olla tarpeen määrittää välitys palvelimen asetukset, kun ne suoritetaan LocalSystem-tieto turva kontekstissa.</span><span class="sxs-lookup"><span data-stu-id="c91fa-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="c91fa-116">Ratkaisu on käyttää Internet Exploreria JÄRJESTELMÄNÄ ja määrittää välitys palvelimen IE:Ä.</span><span class="sxs-lookup"><span data-stu-id="c91fa-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="c91fa-117">Kun Intune Connector-palvelu käynnistetään uudelleen, NDES-yhdistin muodostaa yhteyden Intuneen.</span><span class="sxs-lookup"><span data-stu-id="c91fa-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="c91fa-118">**Käyttäjä laitteet eivät enää saa SCEP-varmenteita NDESIN kautta.**</span><span class="sxs-lookup"><span data-stu-id="c91fa-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="c91fa-119">On mahdollista, että NDES-palvelimelle myönnetty asiakkaan todennus varmenne, joka on määritetty NDES Connector-asennuksen aikana, on vanhentunut tai puuttuu.</span><span class="sxs-lookup"><span data-stu-id="c91fa-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="c91fa-120">Voit korjata ongelman seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="c91fa-120">To resolve:</span></span> 
 
1. <span data-ttu-id="c91fa-121">Poista NDES-yhdistimen asennus.</span><span class="sxs-lookup"><span data-stu-id="c91fa-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="c91fa-122">Näiden tietojen avulla voit pyytää uutta asiakas todentamista tai palvelimen todennus varmennetta:</span><span class="sxs-lookup"><span data-stu-id="c91fa-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="c91fa-123">Aiheen nimi: CN = External täydellinen</span><span class="sxs-lookup"><span data-stu-id="c91fa-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="c91fa-124">Aihe Vaihtoehtoinen nimi (molemmat ovat pakollisia): DNS = External täydellinen, DNS = Internal täydellinen</span><span class="sxs-lookup"><span data-stu-id="c91fa-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="c91fa-125">Asenna NDES-yhdistin uudelleen uuteen sertifikaattiin.</span><span class="sxs-lookup"><span data-stu-id="c91fa-125">Reinstall the NDES connector with the new certificate.</span></span>