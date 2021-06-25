---
title: Sähköpostin välittäminen Microsoft 365:n kautta
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 3b07dd4ccc8570e77a9ce30df48f9ac987a1db71
ms.sourcegitcommit: 93292c46464ac94971d11adfb808d066ab8bc406
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/24/2021
ms.locfileid: "53117980"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="bad02-102">Monitoimilaitteen tai sovelluksen määrittäminen lähettämään sähköpostia</span><span class="sxs-lookup"><span data-stu-id="bad02-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="bad02-103">Tietoja vaihtoehdoista ja toimintavaiheista on artikkelissa [Monitoimilaitteen tai sovelluksen määrittäminen lähettämään sähköpostia Microsoft 365:n avulla](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span><span class="sxs-lookup"><span data-stu-id="bad02-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="bad02-104">Jos jokin laite tai sovellus lakkasi äskettäin toimimasta, yleisimmät ongelmat ovat seuraavat:</span><span class="sxs-lookup"><span data-stu-id="bad02-104">If you have a device or application that recently stopped working, the most common issues are:</span></span>

- <span data-ttu-id="bad02-105">**Todennukseen liittyvät virheet käytettäessä SMTP-todennusta asiakaslähetyksessä** Olemme hiljattain tehneet joitakin SMTP-todennuksen toimintaon liittyviä muutoksia.</span><span class="sxs-lookup"><span data-stu-id="bad02-105">**Authentication related errors while using SMTP Auth client submission** We recently made some changes related to how SMTP Authentication works.</span></span> <span data-ttu-id="bad02-106">Lisätietoja ongelmien ratkaisemisesta on artikkelin Sähköpostin käyttäen sähköpostia Microsoft 365 [](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful)tai Office 365: todennus epäonnistui -osassa.</span><span class="sxs-lookup"><span data-stu-id="bad02-106">For more information about how to resolve issues, see the authentication unsuccessful section of [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).</span></span>
- <span data-ttu-id="bad02-107">**Hyväksymme vain TLS 1.2 -version, kun muodostamme suojatun yhteyden Office 365** Jos käytät suojattua yhteyttä (TLS), varmista, että sovelluslaite tukee TLS 1.2:ta.</span><span class="sxs-lookup"><span data-stu-id="bad02-107">**We accept only the TLS 1.2 version while making a secure connection to Office 365** If you're using Secure connection (TLS), make sure your application device supports TLS 1.2.</span></span> <span data-ttu-id="bad02-108">Lisätietoja on kohdassa [TLS 1.2:n](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)valmistelu Office 365 Office 365 GCC.</span><span class="sxs-lookup"><span data-stu-id="bad02-108">For more information, see [Preparing for TLS 1.2 in Office 365 and Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).</span></span>
 
<span data-ttu-id="bad02-109">Lisätietoja muista ongelmista ja ratkaisuista on kohdassa Sähköpostin sähköpostisovelluksen kautta lähetetyissä tulostimiin, skanneri- ja lobriisisovelluksiin [Microsoft 365 tai Office 365.](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off)</span><span class="sxs-lookup"><span data-stu-id="bad02-109">For other issues and solutions, see [Fix issues with printers, scanners, and LOB applications that send email using Microsoft 365 or Office 365](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).</span></span>

<span data-ttu-id="bad02-110">Jos haluat nähdä, mistä laitteista on kyse, siirry [raporttiin SMTP-todennusta käyttävistä ohjelmista](https://protection.office.com/mailflow/dashboard).</span><span class="sxs-lookup"><span data-stu-id="bad02-110">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span>

<span data-ttu-id="bad02-111">**Huomautus:** Exchange Online ei mahdu joukkopostitusskenaarioihin.</span><span class="sxs-lookup"><span data-stu-id="bad02-111">**Note**: Exchange Online doesn't accommodate bulk-mailing scenarios.</span></span> <span data-ttu-id="bad02-112">Jos haluat lähettää kaupallista joukkosähköpostia (esimerkiksi asiakkaan uutiskirjeitä), käytä näihin palveluihin erikoistamiasi kolmannen osapuolen palveluntarjoajia.</span><span class="sxs-lookup"><span data-stu-id="bad02-112">To send bulk commercial email (for example, customer newsletters), you should use third-party providers that specialize in these services.</span></span>
