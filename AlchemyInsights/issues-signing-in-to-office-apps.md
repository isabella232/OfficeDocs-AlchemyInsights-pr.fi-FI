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
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579934"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="84b15-102">Microsoft 365 -sovellusten "Valitettavasti toinen organisaatiosi tili on jo kirjautunut sisään" -sanoman korjaaminen</span><span class="sxs-lookup"><span data-stu-id="84b15-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="84b15-103">Voit korjata ongelman toimimalla seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="84b15-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="84b15-104">Poista kaikki työtilit, lukuun ottamatta tiliä, jota haavoittuvuus koskee, Windowsin asetusten > **Accessin työpaikalla tai koulussa**.</span><span class="sxs-lookup"><span data-stu-id="84b15-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="84b15-105">[Tyhjennä Officen tunnistetiedot](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windowsin tunnistetietojen hallinnan avulla.</span><span class="sxs-lookup"><span data-stu-id="84b15-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="84b15-106">**Huomautus:** Office 2016:n rekisteripolut ovat muuttuneet 16.0:ksi.</span><span class="sxs-lookup"><span data-stu-id="84b15-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="84b15-107">(Esimerkiksi \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="84b15-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="84b15-108">Avaa Office-sovellus **File**ja valitse  >  **Tiedostotilin**  >  **uloskirjautuminen**. Kirjaudu sitten sisään käyttäjätilillä, jolla on voimassa oleva käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="84b15-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="84b15-109">Saat lisätietoja artikkelista [Office-tilit](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="84b15-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="84b15-110">Jos sinulla on Mac-kone, lue kohta [Kirjautuminen Office 2016 for Mac -sovellukseen ei onnistu](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="84b15-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="84b15-111">Lisätietoja on [Officen kohdassa "Toinen organisaatiosi tili on jo kirjautunut sisään tässä tietokoneessa"](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="84b15-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>