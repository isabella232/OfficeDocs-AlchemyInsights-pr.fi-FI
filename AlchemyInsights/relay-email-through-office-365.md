---
title: Sähköpostin välittäminen Office 365:n kautta
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 9/21/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 84443cf1c93e9b19249c573704bc520eaa1c8f48
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36552965"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email-using-office-365"></a><span data-ttu-id="70497-102">Monitoimilaitteen tai sovelluksen määrittäminen lähettämään sähköpostia Office 365:n avulla</span><span class="sxs-lookup"><span data-stu-id="70497-102">Set up a multifunction device or application to send email using Office 365</span></span>

<span data-ttu-id="70497-103">Tietoja vaihtoehdoista ja toimintavaiheista on artikkelissa [Monitoimilaitteen tai sovelluksen määrittäminen lähettämään sähköpostia Office 365:n avulla](https://support.office.com/article/69f58e99-c550-4274-ad18-c805d654b4c4).</span><span class="sxs-lookup"><span data-stu-id="70497-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Office 365](https://support.office.com/article/69f58e99-c550-4274-ad18-c805d654b4c4).</span></span>
  
<span data-ttu-id="70497-104">**Huomautus:** Jos sinulla on laite tai sovellus, joka on hiljattain lakannut toimimasta, ota huomioon, että [3DES-salaus on poistettu käytöstä](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) äskettäin suunnitelmien mukaan.</span><span class="sxs-lookup"><span data-stu-id="70497-104">**Note:** If you have a device or application which recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="70497-105">Jos haluat nähdä, mistä laitteista on kyse, siirry [raporttiin SMTP-todennusta käyttävistä ohjelmista](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="70497-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="70497-106">Yleisiä virheitä saattavat olla esimerkiksi todennusvirhe, TLS-virhe, salausalgoritmin virhe, algoritmin ristiriita tai yhteyden menettäminen.</span><span class="sxs-lookup"><span data-stu-id="70497-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="70497-107">Ongelman ratkaiseminen:</span><span class="sxs-lookup"><span data-stu-id="70497-107">To resolve the issue:</span></span>
 - <span data-ttu-id="70497-108">**Windows Server 2003 IIS SMTP -palvelu ei enää toimi – tarvitaan uudempi Windows-versio.**</span><span class="sxs-lookup"><span data-stu-id="70497-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="70497-109">Varmista sovelluksen tai laitteen valmistajalta, tuetaanko modernia salausta tai onko tarjolla päivityksiä.</span><span class="sxs-lookup"><span data-stu-id="70497-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
