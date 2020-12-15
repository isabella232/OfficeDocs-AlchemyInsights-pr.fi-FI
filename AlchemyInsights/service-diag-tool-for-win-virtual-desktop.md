---
title: Windowsin Näennäistyöpöytä-palvelun diagnostiikka työkalu
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/14/2020
ms.locfileid: "49678620"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="3e4c2-102">Windowsin Näennäistyöpöytä-palvelun diagnostiikka työkalu</span><span class="sxs-lookup"><span data-stu-id="3e4c2-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="3e4c2-103">Windowsin Näennäistyöpöytä (WVD) tarjoaa diagnostiikka työkalun, jonka avulla järjestelmänvalvojat tunnistavat virheet yksittäisen liittymän kautta.</span><span class="sxs-lookup"><span data-stu-id="3e4c2-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="3e4c2-104">Tämä työkalu kirjaa diagnostiikkaan liittyviä tietoja aina, kun WVD käyttää WVD-roolia.</span><span class="sxs-lookup"><span data-stu-id="3e4c2-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="3e4c2-105">Jokainen loki sisältää tietoja toiminnon WVD-roolista, istunnon aikana ilmestymis virhe sanomista sekä vuokra ajan ja käyttäjän tiedoista.</span><span class="sxs-lookup"><span data-stu-id="3e4c2-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="3e4c2-106">Azure log Analyticsin voi määrittää tallentamaan diagnostiikka työkalun luoman toiminta loki tiedot.</span><span class="sxs-lookup"><span data-stu-id="3e4c2-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="3e4c2-107">Toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="3e4c2-107">Here's how:</span></span>

1. <span data-ttu-id="3e4c2-108">Luo loki analytiikka-työtila [Azure-portaalissa](https://go.microsoft.com/fwlink/?linkid=2129500) tai [Azure PowerShellissä](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="3e4c2-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="3e4c2-109">[Yhdistä Windows-tieto koneet Azure Monitoreen](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="3e4c2-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="3e4c2-110">Hanki työtilan tunnus ja työtilan perusavain.</span><span class="sxs-lookup"><span data-stu-id="3e4c2-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="3e4c2-111">Ohjattu määritys toiminto tarvitsee näitä tietoja, jotta agentti voidaan määrittää oikein ja jotta se voi kommunikoida Azure monitorissa.</span><span class="sxs-lookup"><span data-stu-id="3e4c2-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="3e4c2-112">[Paina diagnostiikan tiedot työtilaan](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="3e4c2-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="3e4c2-113">Voit siirtää diagnostiikan tietoja WVD-vuokra ajasta työtilan loki analytiikkaan.</span><span class="sxs-lookup"><span data-stu-id="3e4c2-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="3e4c2-114">[Tunnista ja diagnosoimaan ongelmia](https://go.microsoft.com/fwlink/?linkid=2128338) , jotka ovat sisäisiä tai ulkoisia suhteessa WVD.</span><span class="sxs-lookup"><span data-stu-id="3e4c2-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="3e4c2-115">Lisä tietoja WVD-palvelun vian määritys työkalun määrittämisestä on artikkelissa [loki analyysin käyttäminen Diagnostiikka-toimintoa varten](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="3e4c2-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
