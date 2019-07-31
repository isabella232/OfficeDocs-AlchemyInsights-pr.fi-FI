---
title: Ongelmia Office-sovellusten kirjautua
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938199"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="5a57e-102">Tyhjä kirjautumisnäytössä Office apps-</span><span class="sxs-lookup"><span data-stu-id="5a57e-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="5a57e-103">Voit korjata tämän ongelman, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="5a57e-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="5a57e-104">Asenna uusimmat päivitykset [Windows](https://support.microsoft.com/help/4027667/windows-10-update) ja [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="5a57e-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="5a57e-105">Palauta Internet Explorerin asetukset: Siirry **Työkalut** > **Internet-asetukset** > **Advanced** > (Huomaa, että menetät mukautetut asetukset)**Palauta Internet Explorerin asetukset** ja yritä sitten kirjautua sisään Office uudelleen.</span><span class="sxs-lookup"><span data-stu-id="5a57e-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="5a57e-106">Poista käytöstä Windows Defender sovelluksen Guard (WDAG) tai vastaava palomuuria tai virustentorjunta ohjelma:</span><span class="sxs-lookup"><span data-stu-id="5a57e-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="5a57e-107">Ohjauspaneelin Siirry **Ohjelmat**ja valitse sitten **Windowsin ominaisuuksien ottaminen käyttöön tai poistaminen käytöstä**.</span><span class="sxs-lookup"><span data-stu-id="5a57e-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="5a57e-108">Jos Windows Defender sovelluksen Guard on käytössä, poista se käytöstä.</span><span class="sxs-lookup"><span data-stu-id="5a57e-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="5a57e-109">**Huomautus:** Saatat joutua käynnistämään tietokoneen uudelleen.</span><span class="sxs-lookup"><span data-stu-id="5a57e-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="5a57e-110">Varmista, että Microsoft.AAD.BrokerPlugin [AAD WAM-laajennus](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) ei ole estää minkä tahansa sovelluksen tai palomuuri tai vastaisten-virus ohjelma.</span><span class="sxs-lookup"><span data-stu-id="5a57e-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="5a57e-111">[Poista Office-tunnistetietoja](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windowsin käyttöoikeuksien hallinnan.</span><span class="sxs-lookup"><span data-stu-id="5a57e-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="5a57e-112">**Huomautus:** Office-2016 Rekisteripolut ovat muuttuneet 16,0.</span><span class="sxs-lookup"><span data-stu-id="5a57e-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="5a57e-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="5a57e-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="5a57e-114">Lisätietoja on kohdassa [yhteyden ongelmia sisään Office 2016 build 16.0.7967 10 Windows-päivityksen jälkeen](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="5a57e-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>