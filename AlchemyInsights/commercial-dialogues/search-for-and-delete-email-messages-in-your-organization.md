---
title: Sähköpostiviestien etsiminen ja poistaminen organisaatiossa
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746432"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="6012d-102">Sähköpostiviestien etsiminen ja poistaminen organisaatiossa</span><span class="sxs-lookup"><span data-stu-id="6012d-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="6012d-103">Toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="6012d-103">Follow these steps:</span></span>

1. <span data-ttu-id="6012d-104">Jos et ole yleinen järjestelmänvalvoja, tilisi on lisättävä **eDiscovery Managerin** rooliryhmään tai yhteensopivuushaun **hallintarooliin,** jotta voit hakea viestejä.</span><span class="sxs-lookup"><span data-stu-id="6012d-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="6012d-105">Jos haluat poistaa viestejä, sinun täytyy liittyä Organisaation hallinta -rooliryhmään **tai** haku- ja **poisto-hallintarooliin.**</span><span class="sxs-lookup"><span data-stu-id="6012d-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="6012d-106">Näiden roolien käyttöoikeudet määritetään tietoturva- & [yhteensopivuuskeskuksessa.](https://protection.office.com)</span><span class="sxs-lookup"><span data-stu-id="6012d-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="6012d-107">[Etsi poistettava viesti](https://docs.microsoft.com/office365/securitycompliance/content-search) luomalla sisältöhaku.</span><span class="sxs-lookup"><span data-stu-id="6012d-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="6012d-108">[Muodosta yhteys tietoturva- & PowerShelliin.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="6012d-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="6012d-109">Jos käytät monimenetelmäistä todentamista, katso seuraavat ohjeet: Muodosta [yhteys tietoturva- & PowerShelliin monimenetelmäisen todentamisen avulla](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="6012d-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="6012d-110">Poista viesti: poista viesti `New-ComplianceSearchAction` suorita cmdlet-komento.</span><span class="sxs-lookup"><span data-stu-id="6012d-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="6012d-111">Poistetut viestit siirretään käyttäjän Palautettavat-kansioon.</span><span class="sxs-lookup"><span data-stu-id="6012d-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="6012d-112">Esimerkkikomento, katso [vaihe 3: Viestin poistaminen.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span><span class="sxs-lookup"><span data-stu-id="6012d-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
