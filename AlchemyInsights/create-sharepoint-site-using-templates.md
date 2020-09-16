---
title: Sivuston luominen SharePoint Onlinessa
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732217"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="620b3-102">SharePoint-sivuston luominen mallien avulla</span><span class="sxs-lookup"><span data-stu-id="620b3-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="620b3-103">Modernia viestintää tai ryhmä sivustoja ei voi käyttää sivuston tallentamiseen mallina.</span><span class="sxs-lookup"><span data-stu-id="620b3-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="620b3-104">Lisä tietoja mallien käyttämisestä on Ohje aiheessa [SharePoint-sivuston tallentaminen, lataaminen ja lataaminen mallina](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="620b3-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="620b3-105">Seuraavassa on joitakin yleisiä ongelmia tai ratkaisuja, jotka liittyvät sivuston tai luettelon tallentamiseen SharePoint Onlinen mallina.</span><span class="sxs-lookup"><span data-stu-id="620b3-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="620b3-106">**Tallenna sivuston/luettelon malli-painike ei ole käytettävissä tai se puuttuu**</span><span class="sxs-lookup"><span data-stu-id="620b3-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="620b3-107">Järjestelmänvalvojien on sallittava malli ominaisuuksien käyttöönotto mukautetulla komento sarjalla.</span><span class="sxs-lookup"><span data-stu-id="620b3-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="620b3-108">Yksityiskohtaisia ohjeita, esimerkkejä ja Huomioitavaa</span><span class="sxs-lookup"><span data-stu-id="620b3-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="620b3-109">Mukautetun komento sarjan salliminen tai estäminen</span><span class="sxs-lookup"><span data-stu-id="620b3-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="620b3-110">Tallenna sivusto mallina-komento ei ole käytettävissä, ja se voi aiheuttaa ongelmia SharePoint Serverin Julkaisuinfrastruktuuria käyttävien sivustojen kanssa.</span><span class="sxs-lookup"><span data-stu-id="620b3-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="620b3-111">**Sivustomallia ei voi luoda tai se ei toimi oikein**</span><span class="sxs-lookup"><span data-stu-id="620b3-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="620b3-112">Mallista saattaa puuttua [ominaisuus](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , eikä se aktivoidu.</span><span class="sxs-lookup"><span data-stu-id="620b3-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="620b3-113">Jos ominaisuus ei ole käytettävissä nykyisessä sivustokokoelmassa, sivustomallia ei voi käyttää sivuston luomiseen.</span><span class="sxs-lookup"><span data-stu-id="620b3-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="620b3-114">Tarkista, ylittävätkö luettelot tai kirjastot 5000-kohteiden [luettelo näkymän raja-arvon](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) , sillä tämä voi estää sivustomallin luomisen.</span><span class="sxs-lookup"><span data-stu-id="620b3-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="620b3-115">Sivustossa saattaa olla käytössä liikaa resursseja, joten sivustomalli ylittää 50 Mt: n rajan.</span><span class="sxs-lookup"><span data-stu-id="620b3-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="620b3-116">Haku saraketta käyttävän luettelon tietojen näyttämisessä on ongelmia.</span><span class="sxs-lookup"><span data-stu-id="620b3-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="620b3-117">Lisä tietoja on Ohje aiheessa [mallin luoma luettelossa ei näy tietoja oikeista haku luettelosta SharePoint Onlinessa](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="620b3-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="620b3-118">Jos haluat lisä tietoja yleisistä ongelmista ja ratkaisuista, valitse [sivustomallien luominen ja käyttäminen](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="620b3-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



