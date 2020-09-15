---
title: Palveluiden käytön keskeytys
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698679"
---
# <a name="access-services-retirement"></a><span data-ttu-id="4f4e6-102">Palveluiden käytön keskeytys</span><span class="sxs-lookup"><span data-stu-id="4f4e6-102">Access services retirement</span></span>

<span data-ttu-id="4f4e6-103">Kuten alun perin ilmoitettiin MC97576, maaliskuussa 2017 ja jatkoi viestintää kuluneen vuoden aikana, palvelu on poistettu käytöstä.</span><span class="sxs-lookup"><span data-stu-id="4f4e6-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="4f4e6-104">Tämän prosessin seuraava vaihe on sellaisten Accessia käyttävien verkko tieto kantojen poistaminen, jotka käyttävät SharePoint-luetteloita pohjana olevien tietojen tallentamiseen.</span><span class="sxs-lookup"><span data-stu-id="4f4e6-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="4f4e6-105">**Miten tämä vaikuttaa minuun?**</span><span class="sxs-lookup"><span data-stu-id="4f4e6-105">**How does this affect me?**</span></span>

<span data-ttu-id="4f4e6-106">Kesä kuun 2019 jälkeen lopetamme uusien tieto kantojen luomisen SharePoint Onlinessa ja suljet palvelun ja kaikki jäljellä olevat sovellukset huhtikuuhun 2020 mennessä.</span><span class="sxs-lookup"><span data-stu-id="4f4e6-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="4f4e6-107">**Mitä minun on tehtävä tämän muutoksen valmistelemiseksi?**</span><span class="sxs-lookup"><span data-stu-id="4f4e6-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="4f4e6-108">Kehotamme sinua luomaan siirtymäsuunnitelmat organisaation verkko tieto kantoja varten.</span><span class="sxs-lookup"><span data-stu-id="4f4e6-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="4f4e6-109">Järjestelmänvalvojat voivat käyttää [SharePoint-sovelluksen sovellus skanneria](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) , joka hankkii luettelon käyttö oikeus sovelluksista, joita sivustot käyttävät.</span><span class="sxs-lookup"><span data-stu-id="4f4e6-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="4f4e6-110">Voit siirtää Accessia koskevia verkko tieto kanta tietoja usealla eri tavalla:</span><span class="sxs-lookup"><span data-stu-id="4f4e6-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="4f4e6-111">Tuominen paikalliseen tieto kantaan (. ACCDB) tai Excel-tiedostoon.</span><span class="sxs-lookup"><span data-stu-id="4f4e6-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="4f4e6-112">Suosittelemme myös tutustumaan Microsoft PowerApps-sovelluksiin vaihtoehtoisena ympäristönä, jotta voit luoda ei-koodi ratkaisuja verkko-ja mobiililaitteisiin.</span><span class="sxs-lookup"><span data-stu-id="4f4e6-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>