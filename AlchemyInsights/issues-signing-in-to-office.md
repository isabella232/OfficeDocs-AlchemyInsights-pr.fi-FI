---
title: Microsoft 365 -sovelluksiin kirjautumiseen liittyvät ongelmat
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
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579898"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="b2e03-102">Tyhjä kirjautumisnäyttö Microsoft 365 -sovelluksissa</span><span class="sxs-lookup"><span data-stu-id="b2e03-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="b2e03-103">Voit korjata tämän ongelman kokeilemalla seuraavaa:</span><span class="sxs-lookup"><span data-stu-id="b2e03-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="b2e03-104">Asenna uusimmat [Windows-](https://support.microsoft.com/help/4027667/windows-10-update) ja [Office-päivitykset](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="b2e03-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="b2e03-105">Internet Explorerin asetusten palauttaminen: Siirry **Työkalut**  >  **Internet-asetukset**Internet  >  **Advanced**  >  **Explorerin asetusten lisäasetukset** -kohtaan (huomaa, että mukautetut asetukset menetetään) ja yritä sitten kirjautua uudelleen Officeen.</span><span class="sxs-lookup"><span data-stu-id="b2e03-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="b2e03-106">Tehdä kykenemättömäksi Akkuna Puoltaa Ahkeruus Junailija (WDAG) eli jokin rinnakkainen polttopuut eli emission- myrkky ohjelmoida:</span><span class="sxs-lookup"><span data-stu-id="b2e03-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="b2e03-107">Valitse Ohjauspaneelissa **Ohjelmat**ja valitse sitten **Ota Windowsin ominaisuudet käyttöön tai poista ne käytöstä**.</span><span class="sxs-lookup"><span data-stu-id="b2e03-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="b2e03-108">Jos Windows Defender Application Guard on käytössä, kokeile poistaa se käytöstä.</span><span class="sxs-lookup"><span data-stu-id="b2e03-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="b2e03-109">**Huomautus:** Tietokone on ehkä käynnistettävä uudelleen.</span><span class="sxs-lookup"><span data-stu-id="b2e03-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="b2e03-110">Varmista, että mikään sovellus tai palomuuri/virustorjuntaohjelma ei estä Microsoft.AAD.BrokerPlugin [AAD WAM -laajennusta.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1)</span><span class="sxs-lookup"><span data-stu-id="b2e03-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="b2e03-111">[Tyhjennä Officen tunnistetiedot](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windowsin tunnistetietojen hallinnan avulla.</span><span class="sxs-lookup"><span data-stu-id="b2e03-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="b2e03-112">**Huomautus:** Office 2016:n rekisteripolut ovat muuttuneet 16.0:ksi.</span><span class="sxs-lookup"><span data-stu-id="b2e03-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="b2e03-113">(Esimerkiksi \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="b2e03-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="b2e03-114">Lisätietoja on [ohjeaiheessa Yhteysongelmat kirjautumisessa Office 2016-koontiversion 16.0.7967 päivittämisen jälkeen Windows 10:ssä](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="b2e03-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>