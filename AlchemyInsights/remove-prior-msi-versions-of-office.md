---
title: Officen aiempien MSI-versioiden poistaminen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003886"
- "6940"
ms.openlocfilehash: 26ab610cb204149536bd23c830a1b8558892a7c0
ms.sourcegitcommit: c033720921cb9a06b9560eedef4f1935e69a846b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2020
ms.locfileid: "49680685"
---
# <a name="remove-prior-msi-versions-of-office"></a><span data-ttu-id="8c8e3-102">Officen aiempien MSI-versioiden poistaminen</span><span class="sxs-lookup"><span data-stu-id="8c8e3-102">Remove prior MSI versions of Office</span></span>

<span data-ttu-id="8c8e3-103">Suosittelen poistamaan Officen aiemmat Windows Installer (MSI)-versiot ennen Office 365 ProPlus-sovelluksen asentamista.</span><span class="sxs-lookup"><span data-stu-id="8c8e3-103">I recommend removing prior Windows Installer (MSI) versions of Office before installing Office 365 ProPlus.</span></span> <span data-ttu-id="8c8e3-104">Voit tehdä tämän seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="8c8e3-104">Here's how to do this:</span></span>

1. <span data-ttu-id="8c8e3-105">Jos olet asentanut Officen MSI-sovelluksen avulla, voit poistaa Officen Officen käyttöönotto työkalulla (ODT).</span><span class="sxs-lookup"><span data-stu-id="8c8e3-105">If you used MSI to install Office, you can use the Office Deployment Tool (ODT) to uninstall Office.</span></span> <span data-ttu-id="8c8e3-106">Voit käyttää Poistamsi-elementtiä **configuration.xml** -tiedostossa.</span><span class="sxs-lookup"><span data-stu-id="8c8e3-106">You can use the RemoveMSI element in your **configuration.xml** file.</span></span>
1. <span data-ttu-id="8c8e3-107">Noudata tämän artikkelin ohjeita: [Office 365-tieto turva & yhteensopivuus keskus.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="8c8e3-107">Follow the instruction in this article: [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span></span>