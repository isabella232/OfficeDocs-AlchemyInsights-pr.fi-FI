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
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938200"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="89dec-102">Vahvistettaessa Office apps ”tietokoneen Luotetut Platform module ei toimi kunnolla”-sanoma</span><span class="sxs-lookup"><span data-stu-id="89dec-102">Fixing the Office apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="89dec-103">Voit korjata tämän virheen, kokeile seuraavaa:</span><span class="sxs-lookup"><span data-stu-id="89dec-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="89dec-104">Asenna uusimmat päivitykset [Windows](https://support.microsoft.com/help/4027667/windows-10-update) ja [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="89dec-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="89dec-105">[Poista Office-tunnistetietoja](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windowsin käyttöoikeuksien hallinnan.</span><span class="sxs-lookup"><span data-stu-id="89dec-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="89dec-106">**Huomautus:** Office-2016 Rekisteripolut ovat muuttuneet 16,0.</span><span class="sxs-lookup"><span data-stu-id="89dec-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="89dec-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="89dec-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="89dec-108">Suorita [korjausohjelma käyttäjän](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) Trusted Platform Module (TPM) virheiden korjaamiseen.</span><span class="sxs-lookup"><span data-stu-id="89dec-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="89dec-109">Määrittää EnableADAL = 0 seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="89dec-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="89dec-110">Napsauta hiiren kakkospainikkeella Windowsin Käynnistä-painiketta, valitse **Suorita**, kirjoita **regedit**ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="89dec-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="89dec-111">Valitse **Kyllä** , jotta Registry Editor tehdä muutoksia laitteen.</span><span class="sxs-lookup"><span data-stu-id="89dec-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="89dec-112">Registry Editor lisätä **EnableADAL** DWORD-arvon, joka on asetettu **0** HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity mukaisesti.</span><span class="sxs-lookup"><span data-stu-id="89dec-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="89dec-113">Lisätietoja on kohdassa [yhteyden ongelmia sisään Office 2016 build 16.0.7967 10 Windows-päivityksen jälkeen](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="89dec-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>