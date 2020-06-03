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
ms.openlocfilehash: 727fa38233697c778caa9325b2671501cb75d5fd
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510713"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="ded6b-102">Monitoimilaitteen tai sovelluksen määrittäminen lähettämään sähköpostia</span><span class="sxs-lookup"><span data-stu-id="ded6b-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="ded6b-103">Tietoja vaihtoehdoista ja toimintavaiheista on artikkelissa [Monitoimilaitteen tai sovelluksen määrittäminen lähettämään sähköpostia Microsoft 365:n avulla](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span><span class="sxs-lookup"><span data-stu-id="ded6b-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-office-3).</span></span>
  
<span data-ttu-id="ded6b-104">**Huomautus:** Jos sinulla on laite tai sovellus, joka on hiljattain lakannut toimimasta, ota huomioon, että [3DES-salaus on poistettu käytöstä](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) äskettäin suunnitelmien mukaan.</span><span class="sxs-lookup"><span data-stu-id="ded6b-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="ded6b-105">Jos haluat nähdä, mistä laitteista on kyse, siirry [raporttiin SMTP-todennusta käyttävistä ohjelmista](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="ded6b-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="ded6b-106">Yleisiä virheitä saattavat olla esimerkiksi todennusvirhe, TLS-virhe, salausalgoritmin virhe, algoritmin ristiriita tai yhteyden menettäminen.</span><span class="sxs-lookup"><span data-stu-id="ded6b-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="ded6b-107">Ongelman ratkaiseminen:</span><span class="sxs-lookup"><span data-stu-id="ded6b-107">To resolve the issue:</span></span>
 - <span data-ttu-id="ded6b-108">**Windows Server 2003 IIS SMTP -palvelu ei enää toimi – tarvitaan uudempi Windows-versio.**</span><span class="sxs-lookup"><span data-stu-id="ded6b-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="ded6b-109">Varmista sovelluksen tai laitteen valmistajalta, tuetaanko modernia salausta tai onko tarjolla päivityksiä.</span><span class="sxs-lookup"><span data-stu-id="ded6b-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
