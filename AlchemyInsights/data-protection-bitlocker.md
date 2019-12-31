---
title: Tieto suoja-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908707"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="54ab6-102">BitLocker-Sala uksen ottaminen käyttöön Intune-avulla</span><span class="sxs-lookup"><span data-stu-id="54ab6-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="54ab6-103">Intune-pääte pisteiden suojaus käytäntöä voidaan käyttää Windows-laitteiden BitLocker-salaus asetusten määrittämiseen.</span><span class="sxs-lookup"><span data-stu-id="54ab6-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="54ab6-104">Lisä tietoja on Ohje aiheessa [Windows 10 (ja uudemmat)-asetukset suojaamaan laitteita Intune-toiminnolla](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="54ab6-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="54ab6-105">Huomaa, että monet uudemmat Windows 10-laitteet tukevat automaattista BitLocker-salausta, joka käynnistyy ilman MDM-käytännön soveltamista.</span><span class="sxs-lookup"><span data-stu-id="54ab6-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="54ab6-106">Tämä saattaa vaikuttaa käytännön soveltamiseen, jos muita kuin oletus asetuksia on määritetty.</span><span class="sxs-lookup"><span data-stu-id="54ab6-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="54ab6-107">Katso lisä tietoja seuraavista usein kysytyistä kysymyksistä.</span><span class="sxs-lookup"><span data-stu-id="54ab6-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="54ab6-108">Lisä tietoja BitLocker-ongelmien vian määrityksestä on kohdassa [Microsoft Intune-työkalun BitLocker-käytäntöjen vian määritys](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="54ab6-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="54ab6-109">**Usein kysytyt kysymykset**</span><span class="sxs-lookup"><span data-stu-id="54ab6-109">**FAQ**</span></span>

 <span data-ttu-id="54ab6-110">K: mitkä Windows-versiot tukevat laitteen salausta pääte pisteiden suojaus käytännön avulla?</span><span class="sxs-lookup"><span data-stu-id="54ab6-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="54ab6-111">V: Intune-pääte pisteen suojaus käytännön asetukset toteutetaan [BitLocker-salaus](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)menetelmän avulla.</span><span class="sxs-lookup"><span data-stu-id="54ab6-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="54ab6-112">Kaikki Windowsin versiot ja koonti versiot eivät tue BitLocker-SALAUS menetelmän versiota.</span><span class="sxs-lookup"><span data-stu-id="54ab6-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="54ab6-113">Tällä hetkellä tuetaan seuraavia Windows-versioita: Enterprise, Education, Mobile, Mobile Enterprise ja Professional (Build 1809 ja uudemmat).</span><span class="sxs-lookup"><span data-stu-id="54ab6-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="54ab6-114">K: Jos laite on jo salattu BitLockerin kanssa käyttämällä käyttö järjestelmän oletus asetuksia salaus menetelmälle ja Sala kirjoituksen voimakkuudesta (XTS-AES-128), Soveltakaamme käytäntöä, jossa eri asetukset laukaisevat automaattisesti aseman uudelleen Sala uksen uusilla asetuksilla?</span><span class="sxs-lookup"><span data-stu-id="54ab6-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="54ab6-115">A: ei.</span><span class="sxs-lookup"><span data-stu-id="54ab6-115">A: No.</span></span> <span data-ttu-id="54ab6-116">Jotta uusi salaus asetus voidaan ottaa käyttöön, asema on ensin purettava.</span><span class="sxs-lookup"><span data-stu-id="54ab6-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="54ab6-117">**Huom:** Jos laite on rekisteröity automaatti ohjaukseen, OOBE-toiminnon aikana tapahtuvaa automaattista salausta ei käynnistetä, ennen kuin Intune-käytäntöä arvioidaan, jolloin käytäntöpohjaisia asetuksia voidaan käyttää käyttö järjestelmän oletus arvojen sijasta.</span><span class="sxs-lookup"><span data-stu-id="54ab6-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="54ab6-118">K: Jos laite salataan Intune-käytännön soveltamisen seura uksena, onko se purettava, kun kyseinen käytäntö poistetaan?</span><span class="sxs-lookup"><span data-stu-id="54ab6-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="54ab6-119">A: Sala ukseen liittyvän käytännön poistaminen ei johda määritettyjen asemien Sala uksen purkamiseen.</span><span class="sxs-lookup"><span data-stu-id="54ab6-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="54ab6-120">K: Miksi Intune-yhteensopivuus käytäntö osoittaa, että laitteeni ei ole BitLocker käytössä, vaikka se on?</span><span class="sxs-lookup"><span data-stu-id="54ab6-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="54ab6-121">V: "BitLocker Enabled"-asetus Intune Compliance-käytännössä hyödyntää Windows Device Health Attestation (DHA)-asiakasta.</span><span class="sxs-lookup"><span data-stu-id="54ab6-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="54ab6-122">Tämä asiakas mittaa vain laitteen tilan käynnistyksen aikana.</span><span class="sxs-lookup"><span data-stu-id="54ab6-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="54ab6-123">Jos laitetta ei ole käynnistetty uudelleen, koska BitLocker-salaus on suoritettu, DHA-asiakas palvelu ei ilmoita BitLocker-Sala uksesta aktiivi seksi.</span><span class="sxs-lookup"><span data-stu-id="54ab6-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 