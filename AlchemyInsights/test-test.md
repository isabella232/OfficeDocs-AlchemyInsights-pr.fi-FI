---
title: SharePoint Online-termi säilöstä puuttuvat termit
ms.author: pebaum
author: Techwriter40
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 0f9efe980987c9ffc64fcf9d5d72a67f0a622867
ms.sourcegitcommit: 23772ebd25a86a879ced40b10566a35e76a79eb5
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/05/2019
ms.locfileid: "36762055"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="d21f0-102">BitLocker-Sala uksen ottaminen käyttöön Intune-avulla</span><span class="sxs-lookup"><span data-stu-id="d21f0-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="d21f0-103">Intune-pääte pisteiden suojaus käytäntöä voidaan käyttää Windows-laitteiden Boitlocker-salaus asetusten määrittämiseen kohdassa: (ja uudemmat) asetukset suojaamaan laitteita Intune-toiminnolla</span><span class="sxs-lookup"><span data-stu-id="d21f0-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="d21f0-104">Huomaa, että monet uudemmat Windows 10-laitteet tukevat automaattista BitLocker-salausta, joka käynnistyy ilman MDM-käytännön soveltamista.</span><span class="sxs-lookup"><span data-stu-id="d21f0-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="d21f0-105">Tämä saattaa vaikuttaa käytännön soveltamiseen, jos muita kuin oletus asetuksia on määritetty.</span><span class="sxs-lookup"><span data-stu-id="d21f0-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="d21f0-106">Katso FAQ lisä tietoja.</span><span class="sxs-lookup"><span data-stu-id="d21f0-106">See FAQ for more detail.</span></span>


<span data-ttu-id="d21f0-107">FAQ  k: mitkä Windows-versiot tukevat laitteen salausta pääte pisteiden suojaus käytännön avulla?</span><span class="sxs-lookup"><span data-stu-id="d21f0-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="d21f0-108"> V: Intune-pääte pisteen suojaus käytännön asetukset toteutetaan BitLocker-SALAUS menetelmän avulla.</span><span class="sxs-lookup"><span data-stu-id="d21f0-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="d21f0-109">Kaikki versiot ja Windows-versiot eivät tue BitLocker-salaus menetelmän tarjoaja. 
     </span><span class="sxs-lookup"><span data-stu-id="d21f0-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="d21f0-110">Tällä kertaa Windows-versiot: Enterprise; Koulutus, mobiili, mobiili yritys ja ammatillinen (rakentaa 1809 eteenpäin) tuetaan.</span><span class="sxs-lookup"><span data-stu-id="d21f0-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="d21f0-111">K: Jos laite on jo salattu BitLockerin kanssa käyttämällä käyttö järjestelmän oletus asetuksia salaus menetelmälle ja Sala kirjoituksen voimakkuudesta (XTS-AES-128) soveltaa käytäntöä, jossa eri asetukset laukaisevat automaattisesti uudelleensalaus aseman uusilla asetuksilla?</span><span class="sxs-lookup"><span data-stu-id="d21f0-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="d21f0-112">A: ei.</span><span class="sxs-lookup"><span data-stu-id="d21f0-112">A: No.</span></span> <span data-ttu-id="d21f0-113">Jotta uudet salaus asetukset voidaan ottaa käyttöön, asema on ensin purettava.</span><span class="sxs-lookup"><span data-stu-id="d21f0-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="d21f0-114">Huomautus Autopilot-toiminnolla rekisteröidyille laitteille automaattista salausta, joka tapahtuisi OOBE-toiminnon aikana, ei käynnistetä, ennen kuin Intune-käytäntöä arvioidaan, jolloin käytäntöpohjaisia asetuksia voidaan käyttää käyttö järjestelmän oletus arvojen sijasta</span><span class="sxs-lookup"><span data-stu-id="d21f0-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="d21f0-115">Q Jos laite on salattu Intune-käytännön soveltamisen seura uksena, salaus puretaan, kun kyseinen käytäntö poistetaan?</span><span class="sxs-lookup"><span data-stu-id="d21f0-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="d21f0-116">A: Sala ukseen liittyvän käytännön poistaminen ei johda määritettyjen asemien Sala uksen purkamiseen.</span><span class="sxs-lookup"><span data-stu-id="d21f0-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="d21f0-117">K: Miksi Intune-yhteensopivuus käytäntö osoittaa, että laitteellasi ei ole "BitLocker käytössä", mutta se on?</span><span class="sxs-lookup"><span data-stu-id="d21f0-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="d21f0-118">V: "BitLocker Enabled"-asetus Intunen yhteensopivuus käytännössä hyödyntää Windows Device Health Attestation (DHA)-asiakasta.</span><span class="sxs-lookup"><span data-stu-id="d21f0-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="d21f0-119">Tämä asiakas mittaa vain laitteen tilan käynnistyksen aikana.</span><span class="sxs-lookup"><span data-stu-id="d21f0-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="d21f0-120">Jos laitetta ei ole käynnistetty uudelleen, koska BitLocker-salaus on suoritettu loppuun, DHA-asiakas palvelu ei ilmoita BitLockerin aktiivi seksi.</span><span class="sxs-lookup"><span data-stu-id="d21f0-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>