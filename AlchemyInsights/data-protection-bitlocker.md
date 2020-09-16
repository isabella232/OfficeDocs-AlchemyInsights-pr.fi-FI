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
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731236"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="4865f-102">BitLocker-Sala uksen ottaminen käyttöön Intunella</span><span class="sxs-lookup"><span data-stu-id="4865f-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="4865f-103">Intune-pääte pisteen suojaus käytäntöä voidaan käyttää Windows-laitteiden BitLocker-salaus asetusten määrittämiseen.</span><span class="sxs-lookup"><span data-stu-id="4865f-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="4865f-104">Lisä tietoja on kohdassa [Windows 10: n (tai uudemman) asetukset laitteiden suojaamiseksi Intune-toiminnolla](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="4865f-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="4865f-105">Huomaa, että monet Windows 10: tä käyttävät uudet laitteet tukevat automaattista BitLocker-salausta, joka käynnistyy ilman MDM-käytäntöä.</span><span class="sxs-lookup"><span data-stu-id="4865f-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="4865f-106">Tämä voi vaikuttaa käytäntöjen soveltamiseen, jos muut kuin oletus asetukset on määritetty.</span><span class="sxs-lookup"><span data-stu-id="4865f-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="4865f-107">Lisä tietoja on seuraavissa usein kysytyissä kysymyksissä.</span><span class="sxs-lookup"><span data-stu-id="4865f-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="4865f-108">Lisä tietoja BitLocker-ongelmien vian määrityksestä on kohdassa [BitLocker-käytäntöjen vian määritys Microsoft Intunella](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="4865f-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="4865f-109">**Usein kysytyt kysymykset**</span><span class="sxs-lookup"><span data-stu-id="4865f-109">**FAQ**</span></span>

 <span data-ttu-id="4865f-110">K: mitkä Windows-versiot tukevat laitteen salausta pääte pisteen suojaus käytäntöä käyttäen?</span><span class="sxs-lookup"><span data-stu-id="4865f-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="4865f-111">A: asetukset Intune-pääte pisteen suojaus käytännössä on toteutettu [BitLocker-salaus menetelmän](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)avulla.</span><span class="sxs-lookup"><span data-stu-id="4865f-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="4865f-112">Kaikki Windowsin versiot eivät tue BitLocker-salaus menetelmän tarjoajaa.</span><span class="sxs-lookup"><span data-stu-id="4865f-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="4865f-113">Tällä hetkellä seuraavat Windows-versiot ovat tuettuja: Enterprise, Education, Mobile, Mobile Enterprise ja Professional (koonti versio 1809 ja uudemmat versiot).</span><span class="sxs-lookup"><span data-stu-id="4865f-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="4865f-114">K: Jos laite on jo salattu BitLocker-Sala uksella käyttämällä käyttö järjestelmän oletus asetuksia salaus menetelmässä ja Sala kirjoituksen voimakkuus (XTS-AES-128), se soveltaa käytäntöä, jossa on käytössä eri asetukset, jolloin uudet asetukset käyttävät aseman uudelleensalausta automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="4865f-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="4865f-115">V: Ei.</span><span class="sxs-lookup"><span data-stu-id="4865f-115">A: No.</span></span> <span data-ttu-id="4865f-116">Jos haluat käyttää uusia cipher-asetuksia, aseman salaus on ensin purettava.</span><span class="sxs-lookup"><span data-stu-id="4865f-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="4865f-117">**Huomautus:** Jos laitteessa on rekisteröity Autopilot, OOBE-toiminnon aikana suoritettava automaattinen salaus ei käynnisty, ennen kuin Intune-käytäntöä arvioidaan, jolloin käytäntöpohjaisia asetuksia voidaan käyttää käyttö järjestelmän oletus arvojen sijasta.</span><span class="sxs-lookup"><span data-stu-id="4865f-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="4865f-118">K: Jos laite salataan Intune-käytännöstä johtuvan sovelluksen avulla, salaus puretaan, kun tämä menettely tapa poistetaan?</span><span class="sxs-lookup"><span data-stu-id="4865f-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="4865f-119">A: salaukseen liittyvän käytäntöjen poistaminen ei johda määritettyjen asemien Sala uksen purkamiseen.</span><span class="sxs-lookup"><span data-stu-id="4865f-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="4865f-120">K: Miksi Intune-yhteensopivuus käytännöt osoittavat, että laitteessani ei ole BitLocker-suojausta käytössä, vaikka se on?</span><span class="sxs-lookup"><span data-stu-id="4865f-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="4865f-121">A: "BitLocker Enabled"-asetus Intune-yhteensopivuus käytännössä käyttää Windows Device Health-ohjelmisto (DHA)-asiakas ohjelmaa.</span><span class="sxs-lookup"><span data-stu-id="4865f-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="4865f-122">Tämä asiakas mittaa vain laitteen tilan käynnistyksen aikana.</span><span class="sxs-lookup"><span data-stu-id="4865f-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="4865f-123">Jos laitetta ei ole käynnistetty uudelleen, koska BitLocker-salaus on valmis, DHA-asiakas palvelu ei ilmoita BitLocker-salausta aktiivi seksi.</span><span class="sxs-lookup"><span data-stu-id="4865f-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 