---
title: Ongelmia, jotka liittyvät Microsoft 365-sovelluksiin kirjautumiseen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695284"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="3c140-102">Microsoft 365-sovellusten tyhjä kirjautumisnäyttö</span><span class="sxs-lookup"><span data-stu-id="3c140-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="3c140-103">Voit korjata ongelman kokeilemalla seuraavaa:</span><span class="sxs-lookup"><span data-stu-id="3c140-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="3c140-104">Asenna [Windowsin](https://support.microsoft.com/help/4027667/windows-10-update) ja [Officen](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)uusimmat päivitykset.</span><span class="sxs-lookup"><span data-stu-id="3c140-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="3c140-105">Internet Explorerin asetusten palauttaminen: Valitse **Työkalut**-  >  kohdan**Internet-asetukset**  >  **Advanced**  >  **Palauta Internet Explorerin asetukset** (Huomaa, että menetät mukautetut asetukset) ja yritä kirja utua uudelleen sisään Officeen.</span><span class="sxs-lookup"><span data-stu-id="3c140-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="3c140-106">Poista Windows Defender Application Guard (WDAG)-sovellus tai muu vastaava palo muuri tai virus torjunta ohjelma käytöstä:</span><span class="sxs-lookup"><span data-stu-id="3c140-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="3c140-107">Valitse ohjaus paneelissa **ohjelmat**ja sitten **Ota Windowsin ominaisuudet käyttöön tai poista ne käytöstä**.</span><span class="sxs-lookup"><span data-stu-id="3c140-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="3c140-108">Jos Windows Defender Application Guard on otettu käyttöön, poista se käytöstä.</span><span class="sxs-lookup"><span data-stu-id="3c140-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="3c140-109">**Huomautus:** Sinun on ehkä käynnistettävä tieto kone uudelleen.</span><span class="sxs-lookup"><span data-stu-id="3c140-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="3c140-110">Varmista, että jokin sovellus tai palo muuri/virus torjunta ohjelma ei estä Microsoft. AAD. BrokerPlugin AAD [WAM-laajennusta](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) .</span><span class="sxs-lookup"><span data-stu-id="3c140-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="3c140-111">[Poista Officen tunniste tiedot käyttämällä Windows Credential](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Manageria.</span><span class="sxs-lookup"><span data-stu-id="3c140-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="3c140-112">**Huomautus:** Office 2016-rekisteri polut ovat muuttuneet 16,0-asetuksiksi.</span><span class="sxs-lookup"><span data-stu-id="3c140-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="3c140-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="3c140-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="3c140-114">Lisä tietoja on kohdassa [kirjautumisen yhteys ongelmat sen jälkeen, kun olet päivittänyt Office 2016-koonti version 16.0.7967 Windows 10: ssä](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="3c140-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>