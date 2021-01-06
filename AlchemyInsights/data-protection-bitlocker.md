---
title: Dataprotectionin-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768814"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="581e9-102">BitLocker-Sala uksen ottaminen käyttöön Intunella</span><span class="sxs-lookup"><span data-stu-id="581e9-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="581e9-103">Intune-pääte pisteen suojaus käytäntöä voidaan käyttää Windows-laitteiden BitLocker-salaus asetusten määrittämiseen.</span><span class="sxs-lookup"><span data-stu-id="581e9-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="581e9-104">Lisä tietoja on kohdassa [Windows 10: n (tai uudemman) asetukset laitteiden suojaamiseksi Intune-toiminnolla](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="581e9-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="581e9-105">Huomaa, että monet Windows 10: tä käyttävät uudet laitteet tukevat automaattista BitLocker-salausta, joka käynnistyy ilman MDM-käytäntöä.</span><span class="sxs-lookup"><span data-stu-id="581e9-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="581e9-106">Tämä voi vaikuttaa käytäntöjen soveltamiseen, jos muut kuin oletus asetukset on määritetty.</span><span class="sxs-lookup"><span data-stu-id="581e9-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="581e9-107">Lisä tietoja on seuraavissa usein kysytyissä kysymyksissä.</span><span class="sxs-lookup"><span data-stu-id="581e9-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="581e9-108">Lisä tietoja BitLocker-ongelmien vian määrityksestä on kohdassa [BitLocker-käytäntöjen vian määritys Microsoft Intunella](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="581e9-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="581e9-109">**Usein kysytyt kysymykset**</span><span class="sxs-lookup"><span data-stu-id="581e9-109">**FAQ**</span></span>

<span data-ttu-id="581e9-110">K: mitkä Windows-versiot tukevat laitteen salausta pääte pisteen suojaus käytäntöä käyttäen?</span><span class="sxs-lookup"><span data-stu-id="581e9-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="581e9-111">A: asetukset Intune-pääte pisteen suojaus käytännössä on toteutettu [BitLocker-salaus menetelmän](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)avulla.</span><span class="sxs-lookup"><span data-stu-id="581e9-111">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="581e9-112">Kaikki Windowsin versiot eivät tue BitLocker-salaus menetelmän tarjoajaa.</span><span class="sxs-lookup"><span data-stu-id="581e9-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="581e9-113">K: Miten BitLocker voidaan ottaa käyttöön laitteissa, jotka eivät edellytä loppu käyttäjän toimia?</span><span class="sxs-lookup"><span data-stu-id="581e9-113">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="581e9-114">A: niin kauan kuin tarvittavat vaatimukset täyttyvät, BitLocker-salaus voidaan ottaa käyttöön Intuneen kautta.</span><span class="sxs-lookup"><span data-stu-id="581e9-114">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="581e9-115">Katso lisä tietoja laitteen vaatimuksista ja esimerkki käytäntöjen asetuksista, jotta hiljainen salaus otetaan käyttöön seuraavassa asia kirjassa: [BitLocker-Sala uksen ottaminen käyttöön](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span><span class="sxs-lookup"><span data-stu-id="581e9-115">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="581e9-116">K: Jos laite on jo salattu BitLocker-Sala uksella käyttämällä käyttö järjestelmän oletus asetuksia salaus menetelmässä ja Sala kirjoituksen voimakkuus (XTS-AES-128), se soveltaa käytäntöä, jossa on käytössä eri asetukset, jolloin uudet asetukset käyttävät aseman uudelleensalausta automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="581e9-116">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="581e9-117">V: Ei.</span><span class="sxs-lookup"><span data-stu-id="581e9-117">A: No.</span></span> <span data-ttu-id="581e9-118">Jos haluat käyttää uusia cipher-asetuksia, aseman salaus on ensin purettava.</span><span class="sxs-lookup"><span data-stu-id="581e9-118">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="581e9-119">**Huomautus:** Jos laitteessa on rekisteröity Autopilot, OOBE-toiminnon aikana suoritettava automaattinen salaus ei käynnisty, ennen kuin Intune-käytäntöä arvioidaan, jolloin käytäntöpohjaisia asetuksia voidaan käyttää käyttö järjestelmän oletus arvojen sijasta.</span><span class="sxs-lookup"><span data-stu-id="581e9-119">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="581e9-120">K: Jos laite salataan Intune-käytännöstä johtuvan sovelluksen avulla, salaus puretaan, kun tämä menettely tapa poistetaan?</span><span class="sxs-lookup"><span data-stu-id="581e9-120">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="581e9-121">A: salaukseen liittyvän käytäntöjen poistaminen ei johda määritettyjen asemien Sala uksen purkamiseen.</span><span class="sxs-lookup"><span data-stu-id="581e9-121">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="581e9-122">K: Miksi Intune-yhteensopivuus käytännöt osoittavat, että laitteessani ei ole BitLocker-suojausta käytössä, vaikka se on?</span><span class="sxs-lookup"><span data-stu-id="581e9-122">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="581e9-123">A: "BitLocker Enabled"-asetus Intune-yhteensopivuus käytännössä käyttää Windows Device Health-ohjelmisto (DHA)-asiakas ohjelmaa.</span><span class="sxs-lookup"><span data-stu-id="581e9-123">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="581e9-124">Tämä asiakas mittaa vain laitteen tilan käynnistyksen aikana.</span><span class="sxs-lookup"><span data-stu-id="581e9-124">This client only measures device state at boot time.</span></span> <span data-ttu-id="581e9-125">Jos laitetta ei ole käynnistetty uudelleen, koska BitLocker-salaus on valmis, DHA-asiakas palvelu ei ilmoita BitLocker-salausta aktiivi seksi.</span><span class="sxs-lookup"><span data-stu-id="581e9-125">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 