---
title: Sivuston tai luettelon tallentaminen mallina
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 7930551c0938501d006f791491594f9d6d9ba260
ms.sourcegitcommit: 56c52c73e752414d66785f175c3a0e2925ad41c1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2019
ms.locfileid: "31044002"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="d8ae3-102">Sivuston tai luettelon tallentaminen mallina</span><span class="sxs-lookup"><span data-stu-id="d8ae3-102">Save site or list as a template</span></span>

<span data-ttu-id="d8ae3-103">SharePoint-sivustomallit ovat suunniteltu tiettyä liiketoiminnan tarvetta valmiista määritelmiä.</span><span class="sxs-lookup"><span data-stu-id="d8ae3-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="d8ae3-104">Lisätietoja [käyttäminen voit luoda SharePoint-sivustoja sekä erilaisia malleja](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="d8ae3-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/en-us/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="d8ae3-105">Seuraavassa on joitakin yleisiä ongelmia ja ratkaisuja koskevat tallentaa sivuston tai luettelon mallina SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="d8ae3-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="d8ae3-106">**Sivustosta/luettelosta Tallenna malli-painike on ei ole käytettävissä tai puuttuu**.</span><span class="sxs-lookup"><span data-stu-id="d8ae3-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="d8ae3-107">Mukautetun komentosarjan avulla on järjestelmänvalvojien käyttöön malliominaisuudet.</span><span class="sxs-lookup"><span data-stu-id="d8ae3-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="d8ae3-108">Saat yksityiskohtaisia ohjeita ja esimerkkejä huomioon otettavia seikkoja [Salli tai estä mukautetun komentosarjan](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="d8ae3-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="d8ae3-109">Tallenna malli-komento sivustoa ei tueta ja julkaiseminen SharePoint Server-infrastruktuuria käyttävien sivustojen käytössä saattaa ilmetä häiriöitä.</span><span class="sxs-lookup"><span data-stu-id="d8ae3-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


**<span data-ttu-id="d8ae3-110">Sivustomalli ei voi luoda tai ei toimi oikein</span><span class="sxs-lookup"><span data-stu-id="d8ae3-110">The site template cannot be created or does not work correctly</span></span>**

- <span data-ttu-id="d8ae3-111">Malli ei ehkä ole [ominaisuus](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ja ei aktivoida.</span><span class="sxs-lookup"><span data-stu-id="d8ae3-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="d8ae3-112">Jos ominaisuus ei ole käytettävissä nykyisen sivustokokoelman aktivoida, ei voi luoda sivuston sivustomallin avulla.</span><span class="sxs-lookup"><span data-stu-id="d8ae3-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="d8ae3-113">Tarkista Jos luetteloita tai kirjastoja enintään 5000 kohteet [Luettelon luettelonäkymän raja](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) tämän sivustomallin luominen voidaan torjua.</span><span class="sxs-lookup"><span data-stu-id="d8ae3-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/en-us/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="d8ae3-114">Sivusto käyttää liikaa resursseja ja näin ollen sivustomalli on enemmän kuin sallitut 50 megatavun (Mt).</span><span class="sxs-lookup"><span data-stu-id="d8ae3-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="d8ae3-115">Ongelmia luettelon, joka sisältää hakusarakkeen tietojen näyttämisen.</span><span class="sxs-lookup"><span data-stu-id="d8ae3-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="d8ae3-116">Lisätietoja [mallin luoma luettelo ei näytä tietoja SharePoint Online-luettelosta oikea valinta](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="d8ae3-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://support.office.com/en-us/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>


<span data-ttu-id="d8ae3-117">Yleisiä ongelmia ja ratkaisuja tarkempia tietoja varten Ota viittaus [sivustomallien luominen ja käyttäminen](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="d8ae3-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/en-us/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

