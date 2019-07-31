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
- "2574"
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938198"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="86e87-102">Ongelmia Office-sovellusten kirjautua</span><span class="sxs-lookup"><span data-stu-id="86e87-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="86e87-103">Kirjautumisongelmien korjaa Office-sovellusten kanssa, yritä seuraavaa:</span><span class="sxs-lookup"><span data-stu-id="86e87-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="86e87-104">Poista kaikki paitsi haavoittuvuuden tilillä, miellyttävät > **käytön tai koulun**työtä tilit.</span><span class="sxs-lookup"><span data-stu-id="86e87-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="86e87-105">[Poista Office-tunnistetietoja](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windowsin käyttöoikeuksien hallinnan.</span><span class="sxs-lookup"><span data-stu-id="86e87-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="86e87-106">**Huomautus:** Office-2016 Rekisteripolut ovat muuttuneet 16,0.</span><span class="sxs-lookup"><span data-stu-id="86e87-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="86e87-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="86e87-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="86e87-108">Avaa Office-sovellus, valitse **Tiedosto** > **huomioon** > **Kirjaudu ulos**. Kirjaudu käyttämällä käyttäjätiliä, jolla on voimassa oleva käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="86e87-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="86e87-109">Yksityiskohtaisia lisätietoja [Office-tilit](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="86e87-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="86e87-110">Katso Mac- [voi kirjautua sisään Mac app for Office 2016](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="86e87-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="86e87-111">Virheiden ilmetessä muodostettaessa yhteyttä Office 365: n käyttäminen Office-2013 käyttöön Nykyaikainen Office-asiakasohjelman todennuksen.</span><span class="sxs-lookup"><span data-stu-id="86e87-111">If the errors occurs while connecting to Office 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="86e87-112">Lisätietoja on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="86e87-112">For more information, see:</span></span>
- [<span data-ttu-id="86e87-113">Et voi kirjautua sisään Office 365 ja Azure Intune</span><span class="sxs-lookup"><span data-stu-id="86e87-113">You can't sign in to Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="86e87-114">Kirjaudu sisään Office 2016-päivityksen jälkeen ongelmia yhteyden rakentaa Windows 10-16.0.7967</span><span class="sxs-lookup"><span data-stu-id="86e87-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="86e87-115">”Valitettavasti organisaatiolta toiselle tilille jo kirjautuneena sisään tähän tietokoneeseen” Office</span><span class="sxs-lookup"><span data-stu-id="86e87-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="86e87-116">Ongelmia sisään Office Moderni todennusta käytettäessä ADFS</span><span class="sxs-lookup"><span data-stu-id="86e87-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)