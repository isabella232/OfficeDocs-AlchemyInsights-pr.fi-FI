---
title: Lähtevien välitysen välitysalue
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381713"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="440da-102">Lähtevien välitysen välitysalue</span><span class="sxs-lookup"><span data-stu-id="440da-102">Outbound relay pool</span></span>

<span data-ttu-id="440da-103">Microsoft tekee joitakin muutoksia sähköpostien välityksen tai edelleenlähetysmäärityksen Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="440da-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="440da-104">Tietyissä tilanteissa viestit välitetään tai välitetään Microsoft 365 erityisen välitystilan avulla.</span><span class="sxs-lookup"><span data-stu-id="440da-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="440da-105">Välityksen avulla lähetetyt viestit voivat päätyä vastaanottajan roskapostikansioon.</span><span class="sxs-lookup"><span data-stu-id="440da-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="440da-106">Lisätietoja on kohdassa Lähtevät [toimituslähteet](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="440da-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="440da-107">Voit välttää skenaarion käyttämällä välityksen välitysä varmistamalla, että välitettyjen/välitettyjen viestien on täytettävä jokin seuraavista ehdoista:</span><span class="sxs-lookup"><span data-stu-id="440da-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="440da-108">Lähtevä lähettäjä on vuokraajan hyväksytty toimialue.</span><span class="sxs-lookup"><span data-stu-id="440da-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="440da-109">SPF (Sender Policy Framework) välittää viestin, kun viesti Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="440da-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="440da-110">P2-lähettäjän toimialueen DomainKeys Identified Mail (DKIM) -näppäin vastaa viestin Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="440da-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="440da-111">Viestejä, jotka täyttävät edellä mainitut ehdot, ei välitetä välityksen kautta.</span><span class="sxs-lookup"><span data-stu-id="440da-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="440da-112">Jos toimialueesi MX-tietue osoittaa kolmannen osapuolen tai paikallisen palvelimen, varmista laajennetun suodatuksen avulla, että SPF-vahvistus on oikea saapuvalle sähköpostille, eikä sähköpostia lähetetä välityksen kautta.</span><span class="sxs-lookup"><span data-stu-id="440da-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="440da-113">**Miten voimme tietää, vaikuttaako välitysalue meitä?**</span><span class="sxs-lookup"><span data-stu-id="440da-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="440da-114">Jos välitetyissä tai välitetyissä sähköpostiviesteissä käytetään jotain edellä mainituista ehdoista, viestejä ei välitetä välityksen kautta.</span><span class="sxs-lookup"><span data-stu-id="440da-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="440da-115">Jos viesti lähetetään välityspalvelimen kautta, lähtevän palvelimen IP-osoite on 40.95.0.0/16-alueella ja lähtevän postin palvelimen nimi **näkyy nimenä rly.**</span><span class="sxs-lookup"><span data-stu-id="440da-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

