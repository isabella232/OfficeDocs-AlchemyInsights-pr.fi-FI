---
title: Kirjautuminen ei onnistu Teamsiin virheen autologon.microsoftazuread-sso.com:443 vuoksi
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931901"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a><span data-ttu-id="9fd36-102">Kirjautuminen ei onnistu Teamsiin virheen autologon.microsoftazuread-sso dot com:443 vuoksi</span><span class="sxs-lookup"><span data-stu-id="9fd36-102">Unable to log into Teams due to error autologon.microsoftazuread-sso dot com:443</span></span>

<span data-ttu-id="9fd36-103">Jos saumaton kertakirjautuminen on otettu käyttöön O365-todennuksena, intranet-sivustoille on ehkä lisättävä URL-osoite ”autologon.microsoftazuread-sso.com”.</span><span class="sxs-lookup"><span data-stu-id="9fd36-103">If Seamless SSO is enabled as the O365 authentication, the URL "autologon.microsoftazuread-sso.com" may need to be added to Intranet Sites.</span></span>  <span data-ttu-id="9fd36-104">Jos se on aiemmin lisätty luotettaville sivustoille ja saumaton kertakirjautuminen on käytössä, se on poistettava luotettavista sivustoista.</span><span class="sxs-lookup"><span data-stu-id="9fd36-104">If it has previously been added to Trusted Sites  and Seamless SSO is in use, it should be removed from Trusted Sites.</span></span>

<span data-ttu-id="9fd36-105">Tarkista [saumattoman kertakirjautumisen vianmäärityksen tarkistusluettelo](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span><span class="sxs-lookup"><span data-stu-id="9fd36-105">Please review the [Seamless SSO Troubleshooting Checklist](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist).</span></span>

<span data-ttu-id="9fd36-106">Voit lisätä URL-osoitteen intranet-sivustojen luetteloon seuraavien ohjeiden mukaisesti:</span><span class="sxs-lookup"><span data-stu-id="9fd36-106">Follow these steps to add a URL to Intranet Sites list:</span></span>

1. <span data-ttu-id="9fd36-107">Avaa Internet Explorer napsauttamalla **Käynnistä**-painiketta.</span><span class="sxs-lookup"><span data-stu-id="9fd36-107">Open Internet Explorer by clicking the **Start** button.</span></span> <span data-ttu-id="9fd36-108">Kirjoita hakukenttään Internet Explorer ja napsauta sitten tulosluettelosta **Internet Explorer**.</span><span class="sxs-lookup"><span data-stu-id="9fd36-108">In the search box, type Internet Explorer, and then, in the list of results, click **Internet Explorer**.</span></span>
2. <span data-ttu-id="9fd36-109">Napsauta **Työkalut** ja napsauta sitten **Internet-asetukset**.</span><span class="sxs-lookup"><span data-stu-id="9fd36-109">Click **Tools**, and then click **Internet options**.</span></span>
3. <span data-ttu-id="9fd36-110">Napsauta **Suojaus**-välilehteä.</span><span class="sxs-lookup"><span data-stu-id="9fd36-110">Click the **Security** tab.</span></span>
4. <span data-ttu-id="9fd36-111">Napsauta nyt **Paikalliset intranet-sivustot** ja napsauta sitten **Sivustot**-painiketta ja sitten **Lisäasetukset**-painiketta.</span><span class="sxs-lookup"><span data-stu-id="9fd36-111">Now click on **Local Intranet sites** and then click on the **sites** button and then **Advanced** button.</span></span>
5. <span data-ttu-id="9fd36-112">Kirjoita verkkosivuston URL-osoite ja napsauta **Lisää**.</span><span class="sxs-lookup"><span data-stu-id="9fd36-112">Enter the Website URL and click **Add**.</span></span>
6. <span data-ttu-id="9fd36-113">Kun olet valmis, napsauta **Sulje**.</span><span class="sxs-lookup"><span data-stu-id="9fd36-113">When you are finished, click **Close**.</span></span>

<span data-ttu-id="9fd36-114">Katso lisätietoja artikkelista [O365:n saumattoman kertakirjautumisen käyttöönotto-ohjeet](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (sisältää käytäntöpohjaisen prosessin URL-osoitteen lisäämiseksi intranet-sivustoille vaiheessa 3).</span><span class="sxs-lookup"><span data-stu-id="9fd36-114">For more information, see [Documentation for deploying Seamless SSO for O365](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (includes Policy-based process to add a URL to Intranet Sites in Step 3).</span></span>
