---
title: Microsoft 365 -sovelluksiin kirjautumisongelmat
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
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709103"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="d6905-102">Tietokoneen luotetun ympäristön moduulin toimimattoman Microsoft 365 -sovellusten korjaamisen sanoma</span><span class="sxs-lookup"><span data-stu-id="d6905-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="d6905-103">Voit korjata ongelman toimimalla seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="d6905-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="d6905-104">Asenna Windowsin ja Officen [uusimmat](https://support.microsoft.com/help/4027667/windows-10-update) [päivitykset.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="d6905-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="d6905-105">[Poista Office-tunnistetiedot](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) Windowsin tunnistetietojen hallinnan avulla.</span><span class="sxs-lookup"><span data-stu-id="d6905-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="d6905-106">**Huomautus:** Office 2016:n rekisteripolut ovat muuttuneet versioksi 16.0.</span><span class="sxs-lookup"><span data-stu-id="d6905-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="d6905-107">(Esim: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="d6905-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="d6905-108">Yritä käyttäjän [palautusprosessia luotettujen](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) ympäristömoduulien (TPM) ongelmien korjaamiseksi.</span><span class="sxs-lookup"><span data-stu-id="d6905-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="d6905-109">Määritä EnableADAL = 0 seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="d6905-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="d6905-110">Napsauta Windowsin Käynnistä-painiketta hiiren kakkospainikkeella, **valitse Suorita,** kirjoita **regedit** ja valitse **sitten OK.**</span><span class="sxs-lookup"><span data-stu-id="d6905-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="d6905-111">Salli **Rekisterieditorin** tehdä muutoksia laitteeseen valitsemalla Kyllä.</span><span class="sxs-lookup"><span data-stu-id="d6905-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="d6905-112">Lisää Rekisterieditorissa **EnableADAL-DWORD-arvo,** jonka asetuksena on **0,** HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="d6905-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="d6905-113">Lisätietoja on kohdassa Kirjautumisongelmat kirjautumisen jälkeen, kun [Windows 10:n Office 2016 -koontiversioon 16.0.7967 on päivitetty.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="d6905-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>