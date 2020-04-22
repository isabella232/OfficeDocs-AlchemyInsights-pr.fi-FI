---
title: Pääsypalvelut eläkkeelle
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
ms.openlocfilehash: 977bd5887ef58b328463a9befcd6b47ac55f5a85
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687255"
---
# <a name="access-services-retirement"></a><span data-ttu-id="83508-102">Pääsypalvelut eläkkeelle</span><span class="sxs-lookup"><span data-stu-id="83508-102">Access services retirement</span></span>

<span data-ttu-id="83508-103">Kuten alun perin ilmoitimme MC97576:ssa maaliskuussa 2017 ja jatkoimme viestintää kuluneen vuoden aikana Access-palvelut ovat eläkkeellä.</span><span class="sxs-lookup"><span data-stu-id="83508-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="83508-104">Tämän prosessin seuraava vaihe on Sellaisten Access Web -tietokantojen poistaminen, jotka käyttävät SharePoint-luetteloita pohjana olevina tietojen tallennina.</span><span class="sxs-lookup"><span data-stu-id="83508-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="83508-105">**Miten tämä vaikuttaa minuun?**</span><span class="sxs-lookup"><span data-stu-id="83508-105">**How does this affect me?**</span></span>

<span data-ttu-id="83508-106">Kesäkuusta 2019 alkaen lopetamme uusien Access-tietokantojen luomisen SharePoint Onlinessa ja suljemme palvelun ja muut jäljellä olevat sovellukset huhtikuuhun 2020 mennessä.</span><span class="sxs-lookup"><span data-stu-id="83508-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="83508-107">**Mitä minun on tehtävä valmistautuakseni tähän muutokseen?**</span><span class="sxs-lookup"><span data-stu-id="83508-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="83508-108">Suosittelemme, että luot siirtymäsuunnitelman organisaation Access-verkkotietokannoille.</span><span class="sxs-lookup"><span data-stu-id="83508-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="83508-109">Järjestelmänvalvojat voivat hankkia [SharePoint Access -sovellusskannerin](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) avulla luettelon sivustoissa käytettävistä Access-sovelluksista.</span><span class="sxs-lookup"><span data-stu-id="83508-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="83508-110">Access-verkkotietokantojen tiedot voidaan siirtää usealla eri tavalla:</span><span class="sxs-lookup"><span data-stu-id="83508-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="83508-111">Tuodaan paikalliseen Access-tietokantaan (. ACCDB) tai Excel-tiedostoon.</span><span class="sxs-lookup"><span data-stu-id="83508-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="83508-112">Microsoft suosittelee myös tutustumaan Microsoft PowerAppsiin vaihtoehtoisena alustana, jotta voit luoda koodittomia liiketoimintaratkaisuja verkko- ja mobiililaitteille.</span><span class="sxs-lookup"><span data-stu-id="83508-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>