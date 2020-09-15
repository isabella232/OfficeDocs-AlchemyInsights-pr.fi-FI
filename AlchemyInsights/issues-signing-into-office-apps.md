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
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695176"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="07a6a-102">Microsoft 365-sovellusten korjaaminen "tieto koneen luotettu käyttö ympäristö moduuli ei toimi oikein"-viesti</span><span class="sxs-lookup"><span data-stu-id="07a6a-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="07a6a-103">Voit korjata ongelman toimimalla seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="07a6a-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="07a6a-104">Asenna [Windowsin](https://support.microsoft.com/help/4027667/windows-10-update) ja [Officen](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)uusimmat päivitykset.</span><span class="sxs-lookup"><span data-stu-id="07a6a-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="07a6a-105">[Poista Officen tunniste tiedot käyttämällä Windows Credential](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Manageria.</span><span class="sxs-lookup"><span data-stu-id="07a6a-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="07a6a-106">**Huomautus:** Office 2016-rekisteri polut ovat muuttuneet 16,0-asetuksiksi.</span><span class="sxs-lookup"><span data-stu-id="07a6a-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="07a6a-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="07a6a-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="07a6a-108">Yritä korjata TPM (Trusted Platform Module)-vikoja kokeilemalla [Käyttäjän palautus prosessia](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) .</span><span class="sxs-lookup"><span data-stu-id="07a6a-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="07a6a-109">Aseta EnableADAL = 0 seuraavien vaiheiden avulla:</span><span class="sxs-lookup"><span data-stu-id="07a6a-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="07a6a-110">Napsauta Windowsin Käynnistä-painiketta hiiren kakkos painikkeella, valitse **Suorita**, kirjoita **regedit**ja valitse sitten **OK**.</span><span class="sxs-lookup"><span data-stu-id="07a6a-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="07a6a-111">Valitse **Kyllä** , jos haluat sallia rekisteri editorin tehdä muutoksia laitteeseesi.</span><span class="sxs-lookup"><span data-stu-id="07a6a-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="07a6a-112">Lisää rekisteri editorissa **Enableadal:n** DWORD-arvo, jonka asetus on **0** , HKEY_CURRENT_USER \Ohjelmatiedostot\office\16.0\common\identty.</span><span class="sxs-lookup"><span data-stu-id="07a6a-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="07a6a-113">Lisä tietoja on kohdassa [kirjautumisen yhteys ongelmat sen jälkeen, kun olet päivittänyt Office 2016-koonti version 16.0.7967 Windows 10: ssä](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="07a6a-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>