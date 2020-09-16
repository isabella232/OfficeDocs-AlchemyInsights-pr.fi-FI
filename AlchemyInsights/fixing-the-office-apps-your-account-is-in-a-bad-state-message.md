---
title: Tilin virheellisen tila viestin korjaaminen Microsoft 365-sovelluksissa
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
- "2558"
- "9000571"
ms.openlocfilehash: ec529291ec9406eba9dc2b0f2cc7a93c77fa3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744542"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="a43a8-102">Microsoft 365-sovellusten korjaaminen "tilisi on väärässä tilassa"-virhe</span><span class="sxs-lookup"><span data-stu-id="a43a8-102">Fixing the Microsoft 365 apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="a43a8-103">Voit korjata tämän virheen kokeilemalla seuraavia vaihto ehtoja haavoittuvuuden sisältävään tieto koneeseen:</span><span class="sxs-lookup"><span data-stu-id="a43a8-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="a43a8-104">Avaa Office-sovellus ja valitse **tiedosto**  >  **tili**  >  **Kirjaudu ulos kaikista tileistäsi**.</span><span class="sxs-lookup"><span data-stu-id="a43a8-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="a43a8-105">Kirjaudu uudelleen sisään käyttämällä käyttäjä tiliä, jolla on voimassa oleva käyttö oikeus.</span><span class="sxs-lookup"><span data-stu-id="a43a8-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="a43a8-106">Saat lisätietoja artikkelista [Office-tilit](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="a43a8-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="a43a8-107">[Poista Officen tunniste tiedot käyttämällä Windows Credential](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Manageria.</span><span class="sxs-lookup"><span data-stu-id="a43a8-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="a43a8-108">**Huomautus:** Office 2016-rekisteri polut ovat muuttuneet 16,0-asetuksiksi.</span><span class="sxs-lookup"><span data-stu-id="a43a8-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="a43a8-109">Esimerkiksi \Software\microsoft\office\16.0\common\identifi-</span><span class="sxs-lookup"><span data-stu-id="a43a8-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="a43a8-110">Jos virhe ilmenee, kun muodostat yhteyden Office 365-palveluun Office 2013-sovelluksen avulla, ota käyttöön Office-asiakas ohjelman [moderni todentaminen](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) .</span><span class="sxs-lookup"><span data-stu-id="a43a8-110">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="a43a8-111">Lisä tietoja on Ohje aiheessa [muiden kuin selain sovellusten, jotka eivät voi kirja utua Microsoft 365-, Azure-tai Intune-sovellukseen, vian määritys](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="a43a8-111">For more information, see [How to troubleshoot non-browser apps that can't sign in to Microsoft  365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

