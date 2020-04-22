---
title: 1049 AntiSpam 4.5.3 Liian monta vastaanottajaa (AS780090)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1049"
- "3100024"
ms.assetid: fa3d4be9-c90a-4926-9754-4b708b038bf6
ms.openlocfilehash: 1afdc8682749a6e9f0c28428e09642269af66f84
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43708016"
---
# <a name="453-too-many-recipients-as780090"></a><span data-ttu-id="e0704-102">4.5.3 Liian monta vastaanottajaa (AS780090)</span><span class="sxs-lookup"><span data-stu-id="e0704-102">4.5.3 Too many recipients (AS780090)</span></span>

<span data-ttu-id="e0704-103">Tämä virhe ilmenee, kun lähde-IP-osoitteen sähköpostiliikenteen määrä ylittää rajoituksen lähde-IP-osoitteen maineen (tai maineen puutteen) perusteella.</span><span class="sxs-lookup"><span data-stu-id="e0704-103">This error occurs when the volume of email traffic from the source IP address exceeds the limit based on the reputation (or lack of reputation) of source IP address.</span></span>

<span data-ttu-id="e0704-104">Sähköpostin estäminen lähde-IP-osoitteesta vanhenee tunnin kuluessa.</span><span class="sxs-lookup"><span data-stu-id="e0704-104">Blocking email from the source IP address will expire within an hour.</span></span> <span data-ttu-id="e0704-105">Jos lähde-IP-osoite on paikallinen sähköpostipalvelin, joka kuuluu sinulle, tarkista postin kulkuliittimen määritys.</span><span class="sxs-lookup"><span data-stu-id="e0704-105">If the source IP address is an on-premises email server that belongs to you, verify the configuration of the mail flow connector.</span></span> <span data-ttu-id="e0704-106">Jos toiminta jatkuu yli tunnin, ota yhteyttä tukeen ja pyydä poikkeusta lähde-IP-osoitteelle.</span><span class="sxs-lookup"><span data-stu-id="e0704-106">If the behavior continues for more than an hour, contact support to request an exception for the source IP address.</span></span>
