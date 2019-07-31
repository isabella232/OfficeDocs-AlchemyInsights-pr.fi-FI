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
- "2560"
ms.openlocfilehash: de0a1b78724db9a8e93d8d599ce3b503abcb86e2
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938197"
---
# <a name="fixing-the-office-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="e0edd-102">Vahvistettaessa Office apps ”valitettavasti jo kirjautuneena toisen tilin organisaatiolta”-sanoma</span><span class="sxs-lookup"><span data-stu-id="e0edd-102">Fixing the Office apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="e0edd-103">Voit korjata tämän virheen, kokeile seuraavaa:</span><span class="sxs-lookup"><span data-stu-id="e0edd-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="e0edd-104">Poista kaikki paitsi haavoittuvuuden tilillä, miellyttävät > **käytön tai koulun**työtä tilit.</span><span class="sxs-lookup"><span data-stu-id="e0edd-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="e0edd-105">[Poista Office-tunnistetietoja](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windowsin käyttöoikeuksien hallinnan.</span><span class="sxs-lookup"><span data-stu-id="e0edd-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="e0edd-106">**Huomautus:** Office-2016 Rekisteripolut ovat muuttuneet 16,0.</span><span class="sxs-lookup"><span data-stu-id="e0edd-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="e0edd-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="e0edd-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="e0edd-108">Avaa Office-sovellus, valitse **Tiedosto** > **huomioon** > **Kirjaudu ulos**. Kirjaudu käyttämällä käyttäjätiliä, jolla on voimassa oleva käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="e0edd-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="e0edd-109">Yksityiskohtaisia lisätietoja [Office-tilit](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="e0edd-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="e0edd-110">Katso Mac- [voi kirjautua sisään Mac app for Office 2016](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="e0edd-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="e0edd-111">Lisätietoja on ohjeaiheessa [”valitettavasti organisaatiolta toiselle tilille jo kirjautuneena sisään tähän tietokoneeseen” Officen](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="e0edd-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>