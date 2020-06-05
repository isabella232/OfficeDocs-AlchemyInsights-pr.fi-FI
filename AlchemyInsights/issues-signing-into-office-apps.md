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
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579862"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="bc0e7-102">Microsoft 365 -sovellusten "Tietokoneen Trusted Platform module ei toimi oikein" -sanoman korjaaminen</span><span class="sxs-lookup"><span data-stu-id="bc0e7-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="bc0e7-103">Voit korjata ongelman toimimalla seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="bc0e7-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="bc0e7-104">Asenna uusimmat [Windows-](https://support.microsoft.com/help/4027667/windows-10-update) ja [Office-päivitykset](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="bc0e7-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="bc0e7-105">[Tyhjennä Officen tunnistetiedot](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windowsin tunnistetietojen hallinnan avulla.</span><span class="sxs-lookup"><span data-stu-id="bc0e7-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="bc0e7-106">**Huomautus:** Office 2016:n rekisteripolut ovat muuttuneet 16.0:ksi.</span><span class="sxs-lookup"><span data-stu-id="bc0e7-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="bc0e7-107">(Esimerkiksi \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="bc0e7-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="bc0e7-108">Yritä korjata Trusted Platform Module (TPM) -virheet [käyttäjän palautusprosessilla.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2)</span><span class="sxs-lookup"><span data-stu-id="bc0e7-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="bc0e7-109">Aseta EnableADAL = 0 seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="bc0e7-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="bc0e7-110">Napsauta Windowsin Käynnistä-painiketta hiiren kakkospainikkeella, valitse **Suorita**, kirjoita **regedit**ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="bc0e7-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="bc0e7-111">Valitse **Kyllä,** jos haluat, että Rekisterieditori voi tehdä muutoksia laitteeseesi.</span><span class="sxs-lookup"><span data-stu-id="bc0e7-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="bc0e7-112">Lisää Rekisterieditorissa **EnableADAL-arvo,** jonka asetus on **0** kohdassa HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="bc0e7-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="bc0e7-113">Lisätietoja on [ohjeaiheessa Yhteysongelmat kirjautumisessa Office 2016-koontiversion 16.0.7967 päivittämisen jälkeen Windows 10:ssä](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="bc0e7-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>