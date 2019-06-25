---
title: SharePoint Online-sivuston luominen
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 9ab06cbd1648da31d8a04e61c237a2326b4bbe93
ms.sourcegitcommit: f856d46a325c517fc29d935c27f21b77c4219e66
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/24/2019
ms.locfileid: "35199270"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="8b2df-102">Luoda SharePoint-sivuston mallien käyttäminen</span><span class="sxs-lookup"><span data-stu-id="8b2df-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="8b2df-103">SharePoint-sivustomallit ovat suunniteltu tiettyä liiketoiminnan tarvetta valmiista määritelmiä.</span><span class="sxs-lookup"><span data-stu-id="8b2df-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="8b2df-104">Lisätietoja [käyttäminen voit luoda SharePoint-sivustoja sekä erilaisia malleja](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="8b2df-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="8b2df-105">Seuraavassa on joitakin yleisiä ongelmia ja ratkaisuja koskevat tallentaa sivuston tai luettelon mallina Sharepoint Online.</span><span class="sxs-lookup"><span data-stu-id="8b2df-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="8b2df-106">**Tallenna sivustosta/luettelosta malli-painike ei ole käytettävissä tai puuttuu**</span><span class="sxs-lookup"><span data-stu-id="8b2df-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="8b2df-107">Mukautetun komentosarjan avulla on järjestelmänvalvojien käyttöön malliominaisuudet.</span><span class="sxs-lookup"><span data-stu-id="8b2df-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="8b2df-108">Lisätietoja esimerkkejä ja huomioista on</span><span class="sxs-lookup"><span data-stu-id="8b2df-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="8b2df-109">Salli tai estä mukautettua komentosarjaa</span><span class="sxs-lookup"><span data-stu-id="8b2df-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="8b2df-110">Tallenna malli-komento sivustoa ei tueta ja julkaiseminen SharePoint Server-infrastruktuuria käyttävien sivustojen käytössä saattaa ilmetä häiriöitä.</span><span class="sxs-lookup"><span data-stu-id="8b2df-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="8b2df-111">**Sivustomalli ei voi luoda tai ei toimi oikein**</span><span class="sxs-lookup"><span data-stu-id="8b2df-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="8b2df-112">Malli ei ehkä ole [ominaisuus](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ja ei aktivoida.</span><span class="sxs-lookup"><span data-stu-id="8b2df-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="8b2df-113">Jos ominaisuus ei ole käytettävissä nykyisen sivustokokoelman aktivoida, ei voi luoda sivuston sivustomallin avulla.</span><span class="sxs-lookup"><span data-stu-id="8b2df-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="8b2df-114">Tarkista Jos luetteloita tai kirjastoja enintään 5000 kohteet [Luettelon luettelonäkymän raja](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) tämän sivustomallin luominen voidaan torjua.</span><span class="sxs-lookup"><span data-stu-id="8b2df-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="8b2df-115">Sivusto käyttää liikaa resursseja ja näin ollen sivustomalli on enemmän kuin sallitut 50 Megatavua.</span><span class="sxs-lookup"><span data-stu-id="8b2df-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="8b2df-116">Ongelmia luettelon, joka sisältää hakusarakkeen tietojen näyttämisen.</span><span class="sxs-lookup"><span data-stu-id="8b2df-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="8b2df-117">Lisätietoja [mallin luoma luettelo ei näytä tietoja SharePoint Online-luettelosta oikea valinta](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span><span class="sxs-lookup"><span data-stu-id="8b2df-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a).</span></span>

<span data-ttu-id="8b2df-118">Yleisiä ongelmia ja ratkaisuja yksityiskohtaisempia tietoja Tarkista [Luo ja käyttää sivustomalleja](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="8b2df-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



