---
title: Käytön rajoittaminen SharePointissa tai OneDrivessa
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692762"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="7542c-102">Käytön rajoittaminen SharePointissa tai OneDrivessa</span><span class="sxs-lookup"><span data-stu-id="7542c-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="7542c-103">SharePoint Onlinen ja OneDrive-palveluiden käyttöä voi rajoittaa monella tavalla.</span><span class="sxs-lookup"><span data-stu-id="7542c-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="7542c-104">Nämä erilaiset käyttörajoitukset on kuvattu alla.</span><span class="sxs-lookup"><span data-stu-id="7542c-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="7542c-105">**Käyttöoikeuksien rajoitus**</span><span class="sxs-lookup"><span data-stu-id="7542c-105">**Permission Restriction**</span></span>

<span data-ttu-id="7542c-106">SharePoint Onlinessa ja OneDrive for Businessissa rajoitamme sivustojen, tiedostojen ja kansioiden kaltaisten kohteiden käyttöä myöntämällä käyttöoikeuden vain niille ryhmille/henkilöille, joilla pitäisi olla käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="7542c-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="7542c-107">SharePoint-luettelon tai -kirjaston käyttöoikeuksien mukauttaminen</span><span class="sxs-lookup"><span data-stu-id="7542c-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="7542c-108">SharePoint-sivuston käyttöoikeuksien mukauttaminen</span><span class="sxs-lookup"><span data-stu-id="7542c-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="7542c-109">Alikansion käyttöoikeuksien muuttaminen</span><span class="sxs-lookup"><span data-stu-id="7542c-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="7542c-110">Hallitsemattomien laitteiden käytön hallinta</span><span class="sxs-lookup"><span data-stu-id="7542c-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="7542c-111">SharePointina tai yleisenä järjestelmänvalvojana voit estää tai rajoittaa SharePoint- ja OneDrive-sisällön käyttöä hallitsemattomista laitteista (jotka eivät ole Intunen yhdistettyjä tai yhteensopivia hybridi-AD:tä).</span><span class="sxs-lookup"><span data-stu-id="7542c-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="7542c-112">**Verkon sijainnin rajoitus**</span><span class="sxs-lookup"><span data-stu-id="7542c-112">**Network Location Restriction**</span></span>

<span data-ttu-id="7542c-113">IT-järjestelmänvalvojana voit hallita SharePoint- ja OneDrive-resurssien käyttöä luotettavien määritettyjen verkkosijaintien perusteella.</span><span class="sxs-lookup"><span data-stu-id="7542c-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="7542c-114">Tätä kutsutaan myös sijaintiin perustuvaksi käytännöksi.</span><span class="sxs-lookup"><span data-stu-id="7542c-114">This is also known as location-based policy.</span></span> <span data-ttu-id="7542c-115">Lisätietoja on ohjeaiheessa [SharePoint Online- ja OneDrive-tietojen käytön hallinta verkkosijainnin perusteella](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="7542c-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="7542c-116">**Sivuston lukituksen rajoitus**</span><span class="sxs-lookup"><span data-stu-id="7542c-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="7542c-117">SharePoint Onlinessa voit lukita sivustokokoelman, joten kenelläkään ei ole käyttöoikeuksia.</span><span class="sxs-lookup"><span data-stu-id="7542c-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="7542c-118">Tämä määritetään PowerShellin ja [SharePoint Online -hallintaliittymän](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) kautta [Set-SPOSite -LockState-ominaisuuden](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) avulla.</span><span class="sxs-lookup"><span data-stu-id="7542c-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="7542c-119">**Käyttäjien estäminen luomasta sivustoja tai alisivustoja**</span><span class="sxs-lookup"><span data-stu-id="7542c-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="7542c-120">SharePoint-järjestelmänvalvojana tai yleisenä järjestelmänvalvojana voit antaa käyttäjien luoda ja hallita omia SharePoint-sivustojaan, määrittää, millaisia sivustoja he voivat luoda, ja määrittää sivustojen sijainnin.</span><span class="sxs-lookup"><span data-stu-id="7542c-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="7542c-121">Lisätietoja on [ohjeaiheessa Sivuston luomisen hallinta SharePoint Onlinessa](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="7542c-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

