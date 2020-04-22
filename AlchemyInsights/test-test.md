---
title: SharePoint Online Term Storesta puuttuvat termit
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766850"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="2b6c8-102">Bitlocker-salauksen ottaminen käyttöön Intunen avulla</span><span class="sxs-lookup"><span data-stu-id="2b6c8-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="2b6c8-103">Intune Endpoint Protection Policy -käytännön avulla voit määrittää Boitlocker-salausasetukset Windows-laitteille kohdassa : Windows10 (ja uudemmat) -asetukset laitteiden suojaamiseksi Intunen avulla</span><span class="sxs-lookup"><span data-stu-id="2b6c8-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="2b6c8-104">Sinun tulisi olla tietoinen siitä, että monet uudemmat laitteet, joissa on Windows 10, tukevat automaattista bitlocker-salausta, joka käynnistyy ilman MDM-käytännön soveltamista.</span><span class="sxs-lookup"><span data-stu-id="2b6c8-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="2b6c8-105">Tämä saattaa vaikuttaa käytännön soveltamiseen, jos muut kuin oletusasetukset on määritetty.</span><span class="sxs-lookup"><span data-stu-id="2b6c8-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="2b6c8-106">Lisätietoja on usein kysytyissä kysymyksissä.</span><span class="sxs-lookup"><span data-stu-id="2b6c8-106">See FAQ for more detail.</span></span>


<span data-ttu-id="2b6c8-107">USEIN  KYSYTYT KYSYMYKSET Q: Mitkä Windows-versiot tukevat laitesalausta päätepisteen suojauskäytännön avulla?</span><span class="sxs-lookup"><span data-stu-id="2b6c8-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="2b6c8-108"> V: Intune Endpoint Protection Policy -käytännön asetukset otetaan käyttöön Bitlockerin CSP-järjestelmän avulla.</span><span class="sxs-lookup"><span data-stu-id="2b6c8-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="2b6c8-109">Kaikki versiot tai Windows-koontiversiot eivät tue Bitlockerin CSP:tä. 
     </span><span class="sxs-lookup"><span data-stu-id="2b6c8-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="2b6c8-110">Tällä hetkellä Windows-versiot: Enterprise; Koulutus, Mobile, Mobile Enterprise ja Professional (alkaen rakentaa 1809 lähtien) ovat tuettuja.</span><span class="sxs-lookup"><span data-stu-id="2b6c8-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="2b6c8-111">K: Jos laite on jo salattu Bitlockerilla käyttäen käyttöjärjestelmän salausmenetelmän ja salakirjoituksen voimakkuutta (XTS-AES-128), sovelletaankäytäntöä, jolla on eri asetukset, käynnistämään aseman uudelleensalauksen automaattisesti uusilla asetuksilla?</span><span class="sxs-lookup"><span data-stu-id="2b6c8-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="2b6c8-112">V: Ei.</span><span class="sxs-lookup"><span data-stu-id="2b6c8-112">A: No.</span></span> <span data-ttu-id="2b6c8-113">Uusien salausasetusten ottamiseksi käyttöön asema on ensin purettava.</span><span class="sxs-lookup"><span data-stu-id="2b6c8-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="2b6c8-114">Huomautus Autopilotilla rekisteröitävien laitteiden automaattinen salaus, joka tapahtuu OOBE:n aikana, ei käynnisty, ennen kuin Intune-käytäntö on arvioitu, jolloin käytäntöpohjaisia asetuksia voidaan käyttää käyttöjärjestelmän oletusasetusten sijasta</span><span class="sxs-lookup"><span data-stu-id="2b6c8-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="2b6c8-115">Q Jos laite on salattu Intune-käytännön soveltamisen seurauksena, puretaanko sen salaus, kun kyseinen käytäntö poistetaan?</span><span class="sxs-lookup"><span data-stu-id="2b6c8-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="2b6c8-116">V: Salaukseen liittyvän käytännön poistaminen EI johda määritettyjen asemien salauksen purkamiseen.</span><span class="sxs-lookup"><span data-stu-id="2b6c8-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="2b6c8-117">K: Miksi intune Compliance -käytäntö osoittaa, että laitteessani ei ole Bitlocker-käyttölaitetta, mutta se on?</span><span class="sxs-lookup"><span data-stu-id="2b6c8-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="2b6c8-118">V: Intune-yhteensopivuuskäytännön Bitlocker-asetus käyttää Windows Device Health Attestation (DHA) -asiakasta.</span><span class="sxs-lookup"><span data-stu-id="2b6c8-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="2b6c8-119">Tämä asiakas mittaa laitteen tilaa vain käynnistyksen aikana.</span><span class="sxs-lookup"><span data-stu-id="2b6c8-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="2b6c8-120">Jos laitetta ei ole käynnistetty uudelleen bitlocker-salauksen valmistuttua, DHA-asiakaspalvelu ei ilmoita bitlockerista aktiiviseksi.</span><span class="sxs-lookup"><span data-stu-id="2b6c8-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>