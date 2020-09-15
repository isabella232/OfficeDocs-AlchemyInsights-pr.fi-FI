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
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695320"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="26685-102">Microsoft 365-sovellusten korjaaminen "Valitettavasti toinen organisaatiosi tili on jo allekirjoitettu" viesti</span><span class="sxs-lookup"><span data-stu-id="26685-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="26685-103">Voit korjata ongelman toimimalla seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="26685-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="26685-104">Poista kaikki työtilit, paitsi heikkouden sisältävä tili, käyttämällä Windowsin asetuksia > **käyttää työpaikan tai oppi laitoksen**tietoja.</span><span class="sxs-lookup"><span data-stu-id="26685-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="26685-105">[Poista Officen tunniste tiedot käyttämällä Windows Credential](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Manageria.</span><span class="sxs-lookup"><span data-stu-id="26685-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="26685-106">**Huomautus:** Office 2016-rekisteri polut ovat muuttuneet 16,0-asetuksiksi.</span><span class="sxs-lookup"><span data-stu-id="26685-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="26685-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="26685-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="26685-108">Avaa Office-sovellus ja valitse **tiedosto**  >  **tili**  >  **Kirjaudu ulos**. Kirjaudu sitten sisään käyttämällä käyttäjä tiliä, jolla on voimassa oleva käyttö oikeus.</span><span class="sxs-lookup"><span data-stu-id="26685-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="26685-109">Saat lisätietoja artikkelista [Office-tilit](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="26685-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="26685-110">Jos sinulla on Mac-kone, lue kohta [Kirjautuminen Office 2016 for Mac -sovellukseen ei onnistu](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="26685-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="26685-111">Lisä tietoja [on kohdassa "Valitettavasti toinen organisaatiosi tili on jo kirjautuneena tähän tieto koneeseen" Officessa](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="26685-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>