---
title: Windowsin virtuaalityöpöydän palveludiagnostiikkatyökalu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595631"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="7392b-102">Windowsin virtuaalityöpöydän palveludiagnostiikkatyökalu</span><span class="sxs-lookup"><span data-stu-id="7392b-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="7392b-103">Windows Virtual Desktop (WVD) tarjoaa diagnostiikkatyökalun, jonka avulla järjestelmänvalvojat voivat tunnistaa virheet yhden käyttöliittymän kautta.</span><span class="sxs-lookup"><span data-stu-id="7392b-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="7392b-104">Tämä työkalu kirjaa diagnostiikkaan liittyvät tiedot aina, kun WVD:lle on määritetty WVD-rooli.</span><span class="sxs-lookup"><span data-stu-id="7392b-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="7392b-105">Jokainen loki sisältää tietoja toiminnon WVD-roolista, istunnon aikana näkyviin tulemista virhesanomista sekä vuokraajan ja käyttäjän tiedot.</span><span class="sxs-lookup"><span data-stu-id="7392b-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="7392b-106">Azure Log Analytics voidaan määrittää sieppaamaan vianmääritystyökalun luoma toimintaloki seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="7392b-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="7392b-107">Luo lokianalyysin työtila [Azure-portaalin tai](https://go.microsoft.com/fwlink/?linkid=2129500) [Azure PowerShellin avulla.](https://go.microsoft.com/fwlink/?linkid=2129501)</span><span class="sxs-lookup"><span data-stu-id="7392b-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="7392b-108">[Yhdistä Windows-tietokoneet Azure Monitoriin.](https://go.microsoft.com/fwlink/?linkid=2129913)</span><span class="sxs-lookup"><span data-stu-id="7392b-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="7392b-109">Hanki työtilan työtilan tunnus ja perusavain.</span><span class="sxs-lookup"><span data-stu-id="7392b-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="7392b-110">Ohjattu määritystoiminto tarvitsee näitä tietoja agenttien määrittämiseen ja sen varmistamiseen, että se voi viestiä Azure Monitorin kanssa.</span><span class="sxs-lookup"><span data-stu-id="7392b-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="7392b-111">[Push diagnostiikkatiedot työtilaan.](https://go.microsoft.com/fwlink/?linkid=2128284)</span><span class="sxs-lookup"><span data-stu-id="7392b-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="7392b-112">Voit käyttää diagnostiikkatietoja WVD-vuokraajassa työtilan lokianalyysiin.</span><span class="sxs-lookup"><span data-stu-id="7392b-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="7392b-113">[Tunnista ja diagnosoi](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) ongelmia, jotka ovat sisäisiä tai ulkoisia WVD:ssä.</span><span class="sxs-lookup"><span data-stu-id="7392b-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="7392b-114">Lisätietoja WVD-palvelun diagnostiikkatyökalun määrittämisestä on kohdassa Lokianalyysin käyttäminen vianmääritystoimintoa varten.</span><span class="sxs-lookup"><span data-stu-id="7392b-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>