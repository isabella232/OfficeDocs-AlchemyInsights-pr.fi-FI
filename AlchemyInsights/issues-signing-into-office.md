---
title: Office-sovelluksiin kirjautumisongelmat
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
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762993"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="e363c-102">Office-sovelluksiin kirjautumisongelmat</span><span class="sxs-lookup"><span data-stu-id="e363c-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="e363c-103">Voit korjata Office-sovellusten kirjautumisongelmat seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="e363c-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="e363c-104">Poista kaikki työtilit, paitsi kyseinen tili, käyttämällä Windowsin asetuksia > **Accessin työ- tai oppilaitokseen**.</span><span class="sxs-lookup"><span data-stu-id="e363c-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="e363c-105">[Tyhjennä Office-tunnistetiedot](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windowsin tunnistetietojen hallinnan avulla.</span><span class="sxs-lookup"><span data-stu-id="e363c-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="e363c-106">**Huomautus:** Office 2016:n rekisteripolut ovat muuttuneet muotoon 16.0.</span><span class="sxs-lookup"><span data-stu-id="e363c-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="e363c-107">(Esim: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="e363c-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="e363c-108">Avaa Office-sovellus ja valitse > **Tiedostotili** > **Kirjaudu ulos**. **File** Kirjaudu sitten sisään käyttäjätilillä, jolla on voimassa oleva käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="e363c-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="e363c-109">Saat lisätietoja artikkelista [Office-tilit](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="e363c-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="e363c-110">Jos sinulla on Mac-kone, lue kohta [Kirjautuminen Office 2016 for Mac -sovellukseen ei onnistu](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="e363c-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="e363c-111">Jos virheet tapahtuvat muodostettaessa yhteyttä Microsoft 365:een Office 2013:n avulla, ota office-asiakasohjelman moderni todennus käyttöön.</span><span class="sxs-lookup"><span data-stu-id="e363c-111">If the errors occurs while connecting to Microsoft 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="e363c-112">Lisätietoja on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="e363c-112">For more information, see:</span></span>
- [<span data-ttu-id="e363c-113">Kirjautuminen Microsoft 365:een, Azureen tai Intuneen ei onnistu</span><span class="sxs-lookup"><span data-stu-id="e363c-113">You can't sign in to Microsoft 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="e363c-114">Yhteysongelmat kirjautumisen yhteydessä Office 2016:n koontiversioon 16.0.7967 Windows 10:ssä</span><span class="sxs-lookup"><span data-stu-id="e363c-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="e363c-115">"Officen toinen tili on jo kirjautunut sisään tähän tietokoneeseen"</span><span class="sxs-lookup"><span data-stu-id="e363c-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="e363c-116">Officen nykyaikaisen todennuksen kirjautumisongelmien vianmääritys ADFS:ää käytettäessä</span><span class="sxs-lookup"><span data-stu-id="e363c-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)