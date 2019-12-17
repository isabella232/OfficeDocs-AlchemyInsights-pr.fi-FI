---
title: Sivuston luominen SharePoint Onlinessa
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 458990889d3c074820527982cbfa6e2d198d3e66
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052466"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="0b4f8-102">SharePoint-sivustojen luominen mallien avulla</span><span class="sxs-lookup"><span data-stu-id="0b4f8-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="0b4f8-103">SharePoint-Sivustomallit ovat ennalta rakennettuja määritelmiä, jotka on suunniteltu tietyn liiketoiminta tarpeen ympärille.</span><span class="sxs-lookup"><span data-stu-id="0b4f8-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="0b4f8-104">Lisä tietoja on kohdassa [mallien käyttäminen erilaisten SharePoint-sivustojen luomiseen](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="0b4f8-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="0b4f8-105">Seuraavassa on joitain yleisiä ongelmia/ratkaisuja, jotka liittyvät sivuston tai luettelon tallentamiseen SharePoint Onlinen mallina.</span><span class="sxs-lookup"><span data-stu-id="0b4f8-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="0b4f8-106">**Tallenna sivusto/luettelo malli-painike ei ole käytettävissä tai puuttuu**</span><span class="sxs-lookup"><span data-stu-id="0b4f8-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="0b4f8-107">Järjestelmänvalvojien on sallittava mukautetun komento sarjan mallin ominaisuuksien ottaminen käyttöön.</span><span class="sxs-lookup"><span data-stu-id="0b4f8-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="0b4f8-108">Tarkempia ohjeita, esimerkkejä ja huomioita on kohdassa</span><span class="sxs-lookup"><span data-stu-id="0b4f8-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="0b4f8-109">Mukautetun komento sarjan salliminen tai estäminen</span><span class="sxs-lookup"><span data-stu-id="0b4f8-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="0b4f8-110">Tallenna sivusto mallina-komentoa ei tueta, ja se voi aiheuttaa ongelmia sivustoissa, jotka käyttävät SharePoint Serverin Julkaisusinfrastruktuuria.</span><span class="sxs-lookup"><span data-stu-id="0b4f8-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="0b4f8-111">**Sivustomallia ei voi luoda tai se ei toimi oikein**</span><span class="sxs-lookup"><span data-stu-id="0b4f8-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="0b4f8-112">Mallista saattaa puuttua [ominaisuus](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) , eikä se aktivoida.</span><span class="sxs-lookup"><span data-stu-id="0b4f8-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="0b4f8-113">Jos ominaisuus ei ole käytettävissä nykyisessä sivustokokoelmassa, et voi käyttää sivustomallia sivuston luomiseen.</span><span class="sxs-lookup"><span data-stu-id="0b4f8-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="0b4f8-114">Tarkista, ylittyessä luettelot tai kirjastot, jotka ylittävät [luettelo näkymän raja-arvon](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) 5000, koska tämä voi estää sivustomallin luomisen.</span><span class="sxs-lookup"><span data-stu-id="0b4f8-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="0b4f8-115">Sivusto saattaa käyttää liikaa resursseja, joten sivustomalli ylittää 50 Mt:N enimmäismäärän.</span><span class="sxs-lookup"><span data-stu-id="0b4f8-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="0b4f8-116">Haku saraketta käyttävän luettelon tietojen näyttämiseen liittyy ongelmia.</span><span class="sxs-lookup"><span data-stu-id="0b4f8-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="0b4f8-117">Lisä tietoja on kohdassa [mallin luoma luettelo ei Näytä tietoja oikeasta haku luettelosta SharePoint Onlinessa](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="0b4f8-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="0b4f8-118">Tarkempia tietoja yleisistä ongelmista ja ratkaisuista, tarkista [Luo ja käytä sivustomalleja](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="0b4f8-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



