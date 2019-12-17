---
title: Rajoita käyttö oikeuksia SharePointissa tai OneDrivessa
ms.author: pebaum
author: pebaum
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 242388af3ae8887616fc123f24502a8e5ac8dfbe
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053762"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="8f952-102">Rajoita käyttö oikeuksia SharePointissa tai OneDrivessa</span><span class="sxs-lookup"><span data-stu-id="8f952-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="8f952-103">SharePoint Online-ja OneDrive-palveluiden käyttöä voi rajoittaa monella tavalla.</span><span class="sxs-lookup"><span data-stu-id="8f952-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="8f952-104">Nämä erilaiset käyttö rajoitus menetelmät on kuvattu alla.</span><span class="sxs-lookup"><span data-stu-id="8f952-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="8f952-105">**Käyttö oikeus rajoitus**</span><span class="sxs-lookup"><span data-stu-id="8f952-105">**Permission Restriction**</span></span>

<span data-ttu-id="8f952-106">SharePoint Onlinessa ja OneDrive for Businessissa rajoitamme sivustojen, tiedostojen ja kansioiden kaltaisten kohteiden käyttöä myöntämällä käyttö oikeudet vain niille ryhmille/henkilöille, joilla pitäisi olla käyttö oikeus.</span><span class="sxs-lookup"><span data-stu-id="8f952-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="8f952-107">SharePoint-luettelon tai-kirjaston käyttö oikeuksien mukauttaminen</span><span class="sxs-lookup"><span data-stu-id="8f952-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="8f952-108">SharePoint-sivuston käyttö oikeuksien mukauttaminen</span><span class="sxs-lookup"><span data-stu-id="8f952-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="8f952-109">Alikansion käyttö oikeuksien muuttaminen</span><span class="sxs-lookup"><span data-stu-id="8f952-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="8f952-110">Hallitsemattomien laitteiden käytön hallinta</span><span class="sxs-lookup"><span data-stu-id="8f952-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="8f952-111">Voit estää tai rajoittaa SharePoint-ja OneDrive-sisällön käyttö oikeuksia hallitsemattoman laitteen SharePoint-tai 365 Global-järjestelmänvalvojana (ei-hybridi mainoksissa, jotka on liitetty tai yhteensopiva Intune-palvelussa).</span><span class="sxs-lookup"><span data-stu-id="8f952-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="8f952-112">**Verkko sijainnin rajoitus**</span><span class="sxs-lookup"><span data-stu-id="8f952-112">**Network Location Restriction**</span></span>

<span data-ttu-id="8f952-113">IT-järjestelmänvalvojana voit hallita SharePoint-ja OneDrive-resurssien käyttöä luotat määritettyjen verkko sijaintien perusteella.</span><span class="sxs-lookup"><span data-stu-id="8f952-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="8f952-114">Tätä kutsutaan myös sijaintipohjaisiksi käytännöiksi.</span><span class="sxs-lookup"><span data-stu-id="8f952-114">This is also known as location-based policy.</span></span> <span data-ttu-id="8f952-115">Lisä tietoja on kohdassa [Hallitse pääsyä SharePoint Onlineen ja OneDrive-tietoihin verkon sijainnin perusteella](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="8f952-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="8f952-116">**Sivuston lukitus rajoitus**</span><span class="sxs-lookup"><span data-stu-id="8f952-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="8f952-117">SharePoint Onlinessa voit lukita sivustokokoelman, joten kukaan ei voi käyttää sitä.</span><span class="sxs-lookup"><span data-stu-id="8f952-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="8f952-118">Tämä asetetaan PowerShellin ja [SharePointin online-hallinta liittymän](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) kautta [Set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate-ominaisuuden avulla.</span><span class="sxs-lookup"><span data-stu-id="8f952-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="8f952-119">**Sivustojen tai alisivustojen luomisen käyttäjien rajoittaminen**</span><span class="sxs-lookup"><span data-stu-id="8f952-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="8f952-120">SharePoint-järjestelmänvalvojana tai Office 365 Global Adminissa voit antaa käyttäjien luoda ja hallinnoida omia SharePoint-sivustoja, määrittää, millaisia sivustoja he voivat luoda ja määrittää sivustojen sijainnin.</span><span class="sxs-lookup"><span data-stu-id="8f952-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="8f952-121">Lisä tietoja on kohdassa [sivuston luomisen hallinta SharePoint Onlinessa](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="8f952-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

