---
title: Microsoft 365 -sovellusten asentaminen Tilisi on virheellinen tila -viestissä
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: 4654b49289a455c1e6641f47fae573d2fcebc717
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812533"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="3e069-102">Microsoft 365 -sovellusten "Tilisi on huonossa tilassa" -virheen asentaminen</span><span class="sxs-lookup"><span data-stu-id="3e069-102">Fixing the Microsoft 365 apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="3e069-103">Voit korjata tämän virheen kokeilemalla seuraavia asetuksia tietokoneessa, johon ongelma vaikuttaa:</span><span class="sxs-lookup"><span data-stu-id="3e069-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="3e069-104">Avaa Office-sovellus ja valitse  >  **Tiedostotili**  >  **Kirjaudu ulos kaikista tileistä.**</span><span class="sxs-lookup"><span data-stu-id="3e069-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="3e069-105">Kirjaudu uudelleen sisään käyttämällä käyttäjätiliä, jolla on kelvollinen käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="3e069-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="3e069-106">Saat lisätietoja artikkelista [Office-tilit](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="3e069-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="3e069-107">[Poista Office-tunnistetiedot](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) Windowsin tunnistetietojen hallinnan avulla.</span><span class="sxs-lookup"><span data-stu-id="3e069-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="3e069-108">**Huomautus:** Office 2016:n rekisteripolut ovat muuttuneet 16.0-versioksi.</span><span class="sxs-lookup"><span data-stu-id="3e069-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="3e069-109">Esimerkiksi \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="3e069-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="3e069-110">Jos virhe ilmenee yhdistettäessä Office 365:een Office 2013:n [avulla,](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) ota moderni todennus käyttöön Office-asiakasohjelmassa.</span><span class="sxs-lookup"><span data-stu-id="3e069-110">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="3e069-111">Lisätietoja on kohdassa Muiden kuin selainsovellusten vianmääritys, jotka eivät voi kirjautua [Microsoft 365:ssä, Azuressa tai Intunessa.](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)</span><span class="sxs-lookup"><span data-stu-id="3e069-111">For more information, see [How to troubleshoot non-browser apps that can't sign in to Microsoft  365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

