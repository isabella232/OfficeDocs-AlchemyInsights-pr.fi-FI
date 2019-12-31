---
title: BitLocker-palautus avaimet
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908812"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="3c954-102">BitLocker-palautus avainten käyttäminen</span><span class="sxs-lookup"><span data-stu-id="3c954-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="3c954-103">Kun määrität BitLocker-asetuksia Intune-pääte pisteen suojaus käytännölle, on mahdollista määrittää, tallennetaanko BitLocker-palautus tiedot Azure Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="3c954-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="3c954-104">Jos tämä asetus on määritetty, tallennettujen palautus tietojen tulee näkyä Intune Adminissa osana Intune Devices Blade-laitteen tietue dataa kahdella tavalla:</span><span class="sxs-lookup"><span data-stu-id="3c954-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="3c954-105">Laitteet-Azure AD Devices-> "laite" tai laitteet-> kaikki laitteet-> "laite"-> palautus avaimet</span><span class="sxs-lookup"><span data-stu-id="3c954-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="3c954-106">Vaihtoehtoisesti, jos sinulla on järjestelmänvalvojan oikeudet itse laitteeseen, palautus avain (sala sana) voidaan nähdä suorittamalla seuraava komento järjestelmänvalvojan oikeuksin suoritettavaan komento kehotteeseen:</span><span class="sxs-lookup"><span data-stu-id="3c954-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
<span data-ttu-id="3c954-107">Jos laite on salattu ennen ilmoittautumista Intunessa, palautus avain on saatettu liittää "Microsoft Account" (MSA)-tiliin, jota käytetään kirjautumiseen laitteeseen OOBE-prosessin aikana.</span><span class="sxs-lookup"><span data-stu-id="3c954-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="3c954-108">Jos näin oli, yhteyden otto https://onedrive.live.com/recoverykey ja kirjautuminen kyseiseen MSA-tieto koneeseen olisi osoitettava laitteet, joihin palautus avaimet on tallennettu.</span><span class="sxs-lookup"><span data-stu-id="3c954-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="3c954-109">Jos laite on salattu kokoonpanon seura uksena toimi alueeseen perustuvan ryhmä käytännön kautta, palautus tiedot voidaan tallentaa paikalliseen Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="3c954-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

