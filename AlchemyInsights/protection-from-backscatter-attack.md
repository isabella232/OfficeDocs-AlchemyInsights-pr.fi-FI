---
title: Suojaus backscatter-hyökkäyksiltä
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9779"
- "9005743"
ms.openlocfilehash: 8d9214fe2f5d55a21c72296421dd837d7f1d7e7d
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035412"
---
# <a name="protection-from-backscatter-attack"></a><span data-ttu-id="b4830-102">Suojaus backscatter-hyökkäyksiltä</span><span class="sxs-lookup"><span data-stu-id="b4830-102">Protection from Backscatter attack</span></span>

<span data-ttu-id="b4830-103">Katkosviestit ovat toimituksen ilmoituksia (ns. NNR-ilmoituksia tai viestin toimituksen toimitusilmoituksia), joita vastaanotat viesteistä, joita et ole lähettänyt.</span><span class="sxs-lookup"><span data-stu-id="b4830-103">Backscatter is non-delivery reports (also known as NDRs or bounce messages) you receive for messages that you did not send.</span></span> <span data-ttu-id="b4830-104">Roskapostin lähettämien estoviestien **vastaanottaja:** viestien osoite, ja ne käyttävät usein oikeita sähköpostiosoitteita uskottavuuden lisäämiseksi viesteilleen.</span><span class="sxs-lookup"><span data-stu-id="b4830-104">Spammers forge (spoof) the **From:** address of their messages, and they often use real email addresses to lend credibility to their messages.</span></span> <span data-ttu-id="b4830-105">Kun roskapostin lähettäjät lähettävät viestejä väistämättä ei-olemassa olevalle vastaanottajalle, kohdesähköpostipalvelinta huijataan palauttamaan NDR-viesti lähettäjälle **Lähettäjä:-osoitteessa.**</span><span class="sxs-lookup"><span data-stu-id="b4830-105">So, when spammers inevitably send messages to non-existent recipients, the destination email server is essentially tricked into returning the undeliverable message in an NDR to the forged sender in the **From:** address.</span></span>

<span data-ttu-id="b4830-106">Lisätietoja on [EOP:n backscatter-kohdassa.](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop)</span><span class="sxs-lookup"><span data-stu-id="b4830-106">Additional Information can be found in [Backscatter in EOP](https://docs.microsoft.com/microsoft-365/security/office-365-security/backscatter-messages-and-eop).</span></span>

<span data-ttu-id="b4830-107">**Taustasuojauksen ottaminen käyttöön**</span><span class="sxs-lookup"><span data-stu-id="b4830-107">**Enabling Backscatter protection**</span></span>

<span data-ttu-id="b4830-108">Jos haluat ottaa käyttöön taustasuojauksen, noudata alla olevaa polkua.</span><span class="sxs-lookup"><span data-stu-id="b4830-108">To enable Backscatter protection, follow the path below.</span></span>

<span data-ttu-id="b4830-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to "On"**</span><span class="sxs-lookup"><span data-stu-id="b4830-109">**protection.office.com > Threat Management > Policy > Antispam > Select the Spam Filter Policy and Edit policy > Spam properties > Mark as spam > NDR backscatter > Set it to “On”**</span></span>

<span data-ttu-id="b4830-110">Jos uskot, että tili on vaarantunut, katso seuraavat:</span><span class="sxs-lookup"><span data-stu-id="b4830-110">If you believe an account has been compromised, see the following:</span></span>

- [<span data-ttu-id="b4830-111">Vaarannun sähköpostitiliin vastaaminen</span><span class="sxs-lookup"><span data-stu-id="b4830-111">Responding to a Compromised Email Account</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/responding-to-a-compromised-email-account)
- [<span data-ttu-id="b4830-112">Estettyjen käyttäjien poistaminen Office 365:n Rajoitetut käyttäjät -portaalista</span><span class="sxs-lookup"><span data-stu-id="b4830-112">Removing blocked users from the Restricted Users portal in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/removing-user-from-restricted-users-portal-after-spam)



