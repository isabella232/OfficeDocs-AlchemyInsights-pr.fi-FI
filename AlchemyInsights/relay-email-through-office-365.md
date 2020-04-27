---
title: Sähköpostin välittäminen Microsoft 365:n kautta
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 4b36caf1841c5292d269812f4ab5ca16a46fbc81
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43785192"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="77e6f-102">Monitoimilaitteen tai sovelluksen määrittäminen lähettämään sähköpostia</span><span class="sxs-lookup"><span data-stu-id="77e6f-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="77e6f-103">Tietoja vaihtoehdoista ja toimintavaiheista on artikkelissa [Monitoimilaitteen tai sovelluksen määrittäminen lähettämään sähköpostia Microsoft 365:n avulla](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span><span class="sxs-lookup"><span data-stu-id="77e6f-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span></span>
  
<span data-ttu-id="77e6f-104">**Huomautus:** Jos sinulla on laite tai sovellus, joka on hiljattain lakannut toimimasta, ota huomioon, että [3DES-salaus on poistettu käytöstä](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) äskettäin suunnitelmien mukaan.</span><span class="sxs-lookup"><span data-stu-id="77e6f-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/office365/securitycompliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="77e6f-105">Jos haluat nähdä, mistä laitteista on kyse, siirry [raporttiin SMTP-todennusta käyttävistä ohjelmista](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="77e6f-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="77e6f-106">Yleisiä virheitä saattavat olla esimerkiksi todennusvirhe, TLS-virhe, salausalgoritmin virhe, algoritmin ristiriita tai yhteyden menettäminen.</span><span class="sxs-lookup"><span data-stu-id="77e6f-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="77e6f-107">Ongelman ratkaiseminen:</span><span class="sxs-lookup"><span data-stu-id="77e6f-107">To resolve the issue:</span></span>
 - <span data-ttu-id="77e6f-108">**Windows Server 2003 IIS SMTP -palvelu ei enää toimi – tarvitaan uudempi Windows-versio.**</span><span class="sxs-lookup"><span data-stu-id="77e6f-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="77e6f-109">Varmista sovelluksen tai laitteen valmistajalta, tuetaanko modernia salausta tai onko tarjolla päivityksiä.</span><span class="sxs-lookup"><span data-stu-id="77e6f-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
