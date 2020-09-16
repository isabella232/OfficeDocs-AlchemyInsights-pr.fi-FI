---
title: Sivuston tai luettelon tallentaminen mallina
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727528"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="bfc7a-102">Sivuston tai luettelon tallentaminen mallina</span><span class="sxs-lookup"><span data-stu-id="bfc7a-102">Save site or list as a template</span></span>

<span data-ttu-id="bfc7a-103">SharePoint-Sivustomallit ovat valmiita määritelmiä, jotka on suunniteltu tietyn yritys tarpeen ympärille.</span><span class="sxs-lookup"><span data-stu-id="bfc7a-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="bfc7a-104">Lisä tietoja on kohdassa [mallien käyttäminen erilaisten SharePoint-sivustotyyppien luomiseen](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="bfc7a-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="bfc7a-105">Seuraavassa on joitakin yleisiä ongelmia tai ratkaisuja, jotka liittyvät sivuston tai luettelon tallentamiseen SharePoint Onlinen mallina.</span><span class="sxs-lookup"><span data-stu-id="bfc7a-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="bfc7a-106">**Tallenna sivuston/luettelon malli-painike ei ole käytettävissä tai se puuttuu**.</span><span class="sxs-lookup"><span data-stu-id="bfc7a-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="bfc7a-107">Järjestelmänvalvojien on sallittava malli ominaisuuksien käyttöönotto mukautetulla komento sarjalla.</span><span class="sxs-lookup"><span data-stu-id="bfc7a-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="bfc7a-108">Yksityiskohtaisia ohjeita, esimerkkejä ja Huomioitavaa on artikkelissa [mukautetun komento sarjan salliminen tai estäminen](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="bfc7a-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="bfc7a-109">Tallenna sivusto mallina-komento ei ole käytettävissä, ja se voi aiheuttaa ongelmia SharePoint Serverin Julkaisuinfrastruktuuria käyttävien sivustojen kanssa.</span><span class="sxs-lookup"><span data-stu-id="bfc7a-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="bfc7a-110">**Sivustomallia ei voi luoda tai se ei toimi oikein**</span><span class="sxs-lookup"><span data-stu-id="bfc7a-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="bfc7a-111">Mallista saattaa puuttua [ominaisuus](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , eikä se aktivoidu.</span><span class="sxs-lookup"><span data-stu-id="bfc7a-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="bfc7a-112">Jos ominaisuus ei ole käytettävissä nykyisessä sivustokokoelmassa, sivustomallia ei voi käyttää sivuston luomiseen.</span><span class="sxs-lookup"><span data-stu-id="bfc7a-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="bfc7a-113">Tarkista, ylittävätkö luettelot tai kirjastot 5000-kohteiden [luettelo näkymän raja-arvon](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) , sillä tämä voi estää sivustomallin luomisen.</span><span class="sxs-lookup"><span data-stu-id="bfc7a-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="bfc7a-114">Sivustossa saattaa olla käytössä liikaa resursseja, joten sivustomalli ylittää 50 Mega tavun (Mt) rajan.</span><span class="sxs-lookup"><span data-stu-id="bfc7a-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="bfc7a-115">Haku saraketta käyttävän luettelon tietojen näyttämisessä on ongelmia.</span><span class="sxs-lookup"><span data-stu-id="bfc7a-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="bfc7a-116">Lisä tietoja on Ohje aiheessa [mallin luoma luettelossa ei näy tietoja oikeista haku luettelosta SharePoint Onlinessa](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="bfc7a-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="bfc7a-117">Lisä tietoja yleisistä ongelmista ja ratkaisuista on Ohje aiheessa [sivustomallien luominen ja käyttäminen](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="bfc7a-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

