---
title: SharePoint Onlinen termi säilöstä puuttuvat ehdot
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750448"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="1cf86-102">BitLocker-Sala uksen ottaminen käyttöön Intunella</span><span class="sxs-lookup"><span data-stu-id="1cf86-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="1cf86-103">Intune-pääte pisteen suoja uksen avulla voit määrittää Boitlocker-salaus asetukset Windows-laitteille kohdassa: Windows10 (ja uudemmat) asetukset, jotka suojaavat laitteita Intunea käyttäen</span><span class="sxs-lookup"><span data-stu-id="1cf86-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="1cf86-104">Huomaa, että monet Windows 10: tä käyttävät uudet laitteet tukevat automaattista BitLocker-salausta, joka käynnistyy ilman MDM-käytäntöä.</span><span class="sxs-lookup"><span data-stu-id="1cf86-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="1cf86-105">Tämä voi vaikuttaa käytäntöjen soveltamiseen, jos muut kuin oletus asetukset on määritetty.</span><span class="sxs-lookup"><span data-stu-id="1cf86-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="1cf86-106">Katso lisä tietoja usein kysytyistä kysymyksistä.</span><span class="sxs-lookup"><span data-stu-id="1cf86-106">See FAQ for more detail.</span></span>


<span data-ttu-id="1cf86-107">Usein kysytyt kysymykset   k: mitkä Windows-versiot tukevat laitteen salausta pääte pisteen suojaus käytäntöä käyttäen?</span><span class="sxs-lookup"><span data-stu-id="1cf86-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="1cf86-108"> A: asetukset Intune-pääte pisteen suojaus käytännössä on toteutettu BitLocker-salaus menetelmän avulla.</span><span class="sxs-lookup"><span data-stu-id="1cf86-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="1cf86-109">Kaikki versiot eivät tue BitLocker-salaus menetelmän tarjoajaa. 
     </span><span class="sxs-lookup"><span data-stu-id="1cf86-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="1cf86-110">Tällä hetkellä Windows-versiot: Enterprise; Koulutus, matka Puhelin, mobiilisovellus ja Professional (koonti versio 1809 alkaen) ovat tuettuja.</span><span class="sxs-lookup"><span data-stu-id="1cf86-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="1cf86-111">K: Jos laite on jo salattu BitLocker-Sala uksella käyttämällä käyttö järjestelmän oletus asetuksia salaus menetelmässä ja Sala kirjoituksen voimakkuus (XTS-AES-128), käytetään käytäntöä, jossa on eri asetukset, jotka automaattisesti käyttävät aseman uudelleensalausta uusilla asetuksilla?</span><span class="sxs-lookup"><span data-stu-id="1cf86-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="1cf86-112">V: Ei.</span><span class="sxs-lookup"><span data-stu-id="1cf86-112">A: No.</span></span> <span data-ttu-id="1cf86-113">Uuden salaus asetuksen käyttäminen edellyttää, että aseman salaus on ensin purettava.</span><span class="sxs-lookup"><span data-stu-id="1cf86-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="1cf86-114">Huomautus OOBE-toiminnon aikana käyttöön otetuista laitteista ei käynnistetä automaattista salausta, ennen kuin Intune-käytäntöä arvioidaan, jolloin käytäntöpohjaisia asetuksia voidaan käyttää käyttö järjestelmän oletus asetusten sijasta.</span><span class="sxs-lookup"><span data-stu-id="1cf86-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="1cf86-115">K jos laite salataan Intune-käytäntöjen soveltamisen seura uksena, salaus puretaan, kun tämä menettely tapa poistetaan?</span><span class="sxs-lookup"><span data-stu-id="1cf86-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="1cf86-116">A: Sala ukseen liittyvän käytäntöjen poistaminen ei johda määritettyjen asemien Sala uksen purkamiseen.</span><span class="sxs-lookup"><span data-stu-id="1cf86-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="1cf86-117">K: Miksi Intune-yhteensopivuus käytännöt osoittavat, että laitteessani ei ole "BitLocker käytössä", mutta se on?</span><span class="sxs-lookup"><span data-stu-id="1cf86-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="1cf86-118">A: "BitLocker Enabled"-asetus Intune-yhteensopivuus käytännössä hyödyntää Windows Device Health-tieto asema (DHA)-asiakas ohjelmaa.</span><span class="sxs-lookup"><span data-stu-id="1cf86-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="1cf86-119">Tämä asiakas mittaa vain laitteen tilan käynnistyksen aikana.</span><span class="sxs-lookup"><span data-stu-id="1cf86-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="1cf86-120">Jos laitetta ei ole käynnistetty uudelleen, koska BitLocker-salaus on valmis, DHA-asiakas palvelu ei ilmoita BitLocker-salausta aktiivi seksi.</span><span class="sxs-lookup"><span data-stu-id="1cf86-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>