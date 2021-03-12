---
title: MDATP-asennusongelmien vianmääritys Macissa
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746305"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="1cb69-102">MDATP-asennusongelmien vianmääritys Macissa</span><span class="sxs-lookup"><span data-stu-id="1cb69-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="1cb69-103">Jos manuaalinen asennus epäonnistuu, **ohjatun** asennuksen yhteenvetosivulla näkyy seuraava virhe:</span><span class="sxs-lookup"><span data-stu-id="1cb69-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="1cb69-104">"Asennuksen aikana tapahtui virhe.</span><span class="sxs-lookup"><span data-stu-id="1cb69-104">"An error occurred during installation.</span></span> <span data-ttu-id="1cb69-105">Asennusohjelma kohtasi virheen, joka aiheutti asennuksen epäonnistumisen.</span><span class="sxs-lookup"><span data-stu-id="1cb69-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="1cb69-106">Pyydä apua ohjelmistovalmistajalta."</span><span class="sxs-lookup"><span data-stu-id="1cb69-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="1cb69-107">MDM-käyttöönotoissa sivulla näkyy myös yleinen asennusvirhe.</span><span class="sxs-lookup"><span data-stu-id="1cb69-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="1cb69-108">Vaikka emme näytä tarkkoja virheitä loppukäyttäjille, säilytämme lokitiedoston asennuksen edistymisen kanssa **kohteessa /Library/Logs/Microsoft/mdatp/install.log.**</span><span class="sxs-lookup"><span data-stu-id="1cb69-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="1cb69-109">Jokainen asennusistunto liitetään tähän lokitiedostoon.</span><span class="sxs-lookup"><span data-stu-id="1cb69-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="1cb69-110">Jos haluat tulostaa vain viimeisen asennusistunnon, käytä `sed` .</span><span class="sxs-lookup"><span data-stu-id="1cb69-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="1cb69-111">Lisätietoja on kohdassa [Microsoft Defender ATP for Macin asennusongelmien vianmääritys.](https://go.microsoft.com/fwlink/?linkid=2144615)</span><span class="sxs-lookup"><span data-stu-id="1cb69-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
