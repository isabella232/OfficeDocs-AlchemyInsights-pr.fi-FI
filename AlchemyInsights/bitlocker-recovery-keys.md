---
title: Bitlocker-palautusavaimet
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820283"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="bf927-102">BitLocker-palautusavainten käyttäminen</span><span class="sxs-lookup"><span data-stu-id="bf927-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="bf927-103">Kun määrität BitLocker-asetuksia Intune Endpoint Protection Policy -palvelussa, on mahdollista määrittää, tallennetaanko Bitlocker-palautustiedot Azure Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="bf927-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="bf927-104">Jos tämä asetus on määritetty, tallennettujen palautustietojen pitäisi näkyä Intune-järjestelmänvalvojalle osana laitteen tietuetietoja Intune-laitteissa kahdella tavalla:</span><span class="sxs-lookup"><span data-stu-id="bf927-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="bf927-105">Laitteet - Azure AD -laitteet > "Laite" TAI Laitteet -> Kaikki laitteet -> "Laite" -> palautusavaimet</span><span class="sxs-lookup"><span data-stu-id="bf927-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="bf927-106">Jos itse laitteella on järjestelmänvalvojan käyttöoikeudet, palautusavain (salasana) voidaan nähdä suorittamalla seuraava komento järjestelmänvalvojan oikeuksin oikeutetussa komentokehotteessa:</span><span class="sxs-lookup"><span data-stu-id="bf927-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="bf927-107">Jos laite on salattu ennen intune-salausta, palautusavain on ehkä liitetty Microsoft-tiliin (MSA), jota käytetään laitteeseen kirjautumisessa OOBE-prosessin aikana.</span><span class="sxs-lookup"><span data-stu-id="bf927-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="bf927-108">Tässä tapauksessa MSA:n käytön ja sisäänkirjautumisen pitäisi näyttää  https://onedrive.live.com/recoverykey laitteet, joiden palautusavaimet on tallennettu.</span><span class="sxs-lookup"><span data-stu-id="bf927-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="bf927-109">Jos laite on salattu toimialuepohjaisen ryhmäkäytännön tuloksena, palautustiedot saatetaan tallentaa paikalliseen Active Directoryyn.</span><span class="sxs-lookup"><span data-stu-id="bf927-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="bf927-110">Jos olet määrittänyt Endpoint-suojauskäytännön, joka tallentaa palautusavaimen Azure Active Directoryyn, mutta tietyn laitteen avainta ei ole ladattu, voit käynnistää latauksen kiertämällä palautusavaimen laitteesta MEM-konsolista.</span><span class="sxs-lookup"><span data-stu-id="bf927-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="bf927-111">Lisätietoja on kohdassa [BitLocker-palautusavainten kiertäminen.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)</span><span class="sxs-lookup"><span data-stu-id="bf927-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

