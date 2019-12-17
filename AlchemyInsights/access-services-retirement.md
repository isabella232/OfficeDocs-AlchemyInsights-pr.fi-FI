---
title: Pääsy palveluiden eläkkeelle
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: cb8123583b68e945ef878fdbaf211fd1d8205bb3
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050486"
---
# <a name="access-services-retirement"></a><span data-ttu-id="d39d8-102">Pääsy palveluiden eläkkeelle</span><span class="sxs-lookup"><span data-stu-id="d39d8-102">Access services retirement</span></span>

<span data-ttu-id="d39d8-103">Kuten alun perin ilmoitettiin MC97576, maaliskuussa 2017, ja jatkoi kommunikointi kuluneen vuoden aikana pääsy palvelut poistetaan käytöstä Office 365.</span><span class="sxs-lookup"><span data-stu-id="d39d8-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="d39d8-104">Tämän prosessin seuraava vaihe on sellaisten Access-Web-tieto kantojen poistaminen, jotka käyttävät SharePoint-luetteloita pohjana olevaan tietojen tallennukseen.</span><span class="sxs-lookup"><span data-stu-id="d39d8-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="d39d8-105">**Miten tämä vaikuttaa minuun?**</span><span class="sxs-lookup"><span data-stu-id="d39d8-105">**How does this affect me?**</span></span>

<span data-ttu-id="d39d8-106">Kesä kuun 2019 alkaen, emme lopeta uusien Access-tieto kantojen luomista SharePoint Onlinessa ja Sammuta palvelu ja mahdolliset jäljellä olevat sovellukset huhtikuun 2020 mennessä.</span><span class="sxs-lookup"><span data-stu-id="d39d8-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="d39d8-107">**Mitä minun täytyy tehdä valmistautuaksemme tähän muutokseen?**</span><span class="sxs-lookup"><span data-stu-id="d39d8-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="d39d8-108">Kehotamme sinua luomaan organisaation Access-Web-tieto kantoihin siirtymis suunnitelman.</span><span class="sxs-lookup"><span data-stu-id="d39d8-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="d39d8-109">Järjestelmänvalvojat voivat käyttää [SharePoint Access-sovelluksen skanneria](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) hankkiakseen inventaarion sivustojen käyttämistä sovelluksista.</span><span class="sxs-lookup"><span data-stu-id="d39d8-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="d39d8-110">Access-Web-tieto kantojen tietoja voi siirtää usealla eri tavalla:</span><span class="sxs-lookup"><span data-stu-id="d39d8-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="d39d8-111">Tuodaan paikalliseen Access-tieto kantaan (. ACCDB) tai Excel-tiedostoon.</span><span class="sxs-lookup"><span data-stu-id="d39d8-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="d39d8-112">Suosittelemme myös tutustumaan Microsoft Powerappsiin vaihtoehtoisena foorumina, joka luo ei-koodaavia liiketoiminta ratkaisuja verkko-ja mobiililaitteille.</span><span class="sxs-lookup"><span data-stu-id="d39d8-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>