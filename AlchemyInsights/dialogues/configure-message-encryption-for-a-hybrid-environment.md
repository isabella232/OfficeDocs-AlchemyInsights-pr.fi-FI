---
title: Viestin salauksen määrittäminen yhdistelmäympäristössä
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 22c2468b7639680b447b6464431a79b69f7198c3
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524825"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a><span data-ttu-id="71eb5-102">Viestin salauksen määrittäminen yhdistelmäympäristössä</span><span class="sxs-lookup"><span data-stu-id="71eb5-102">Configure message encryption for a hybrid environment</span></span>

<span data-ttu-id="71eb5-103">Exchange-yhdistelmäympäristöissä paikallinen käyttäjä voi lähettää salattua sähköpostia Office Message Encryption (OME) -salauksella vain, jos sähköposti reititetaan Exchange Onlinen kautta.</span><span class="sxs-lookup"><span data-stu-id="71eb5-103">For hybrid Exchange environments, on-premises users can send encrypted email using Office Message Encryption (OME) only if email is routed through Exchange Online.</span></span>

<span data-ttu-id="71eb5-104">Voit salata sähköpostiviestit OME:n avulla seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="71eb5-104">To encrypt emails using OME, perform the following steps:</span></span>

1. <span data-ttu-id="71eb5-105">Määritä [yhdistelmäympäristö ohjatun](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) yhdistelmäympäristön määritystoiminnon avulla.</span><span class="sxs-lookup"><span data-stu-id="71eb5-105">Use the [Hybrid Configuration wizard](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) to set up your hybrid environment.</span></span> <span data-ttu-id="71eb5-106">Salauksen määrittämiseen ei tarvita erityisiä vaiheita.</span><span class="sxs-lookup"><span data-stu-id="71eb5-106">No special steps are required for setting up encryption.</span></span>
2. <span data-ttu-id="71eb5-107">[Määritä postinkulkusäännöt salausta](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) varten normaaliin tapaan.</span><span class="sxs-lookup"><span data-stu-id="71eb5-107">[Set up your mail flow rules for encryption](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) like you normally would.</span></span>


