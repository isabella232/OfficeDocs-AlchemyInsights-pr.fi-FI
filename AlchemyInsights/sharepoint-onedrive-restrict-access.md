---
title: Käytön rajoittaminen SharePointissa tai OneDrivessa
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700452"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="eac9b-102">Käytön rajoittaminen SharePointissa tai OneDrivessa</span><span class="sxs-lookup"><span data-stu-id="eac9b-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="eac9b-103">SharePoint Online-ja OneDrive-palveluiden käyttöä voi rajoittaa monin eri tavoin.</span><span class="sxs-lookup"><span data-stu-id="eac9b-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="eac9b-104">Seuraavat eri käytön rajoitus tavat on kuvattu alla.</span><span class="sxs-lookup"><span data-stu-id="eac9b-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="eac9b-105">**Käyttö oikeus rajoitus**</span><span class="sxs-lookup"><span data-stu-id="eac9b-105">**Permission Restriction**</span></span>

<span data-ttu-id="eac9b-106">SharePoint Onlinessa ja OneDrive for Businessissa rajoitetaan kohteiden, kuten sivuston, tiedostojen ja kansioiden, käyttöä myöntämällä vain niiden ryhmien/henkilöiden oikeudet, joilla on oikeus käyttää niitä.</span><span class="sxs-lookup"><span data-stu-id="eac9b-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="eac9b-107">SharePoint-luettelon tai-kirjaston käyttö oikeuksien mukauttaminen</span><span class="sxs-lookup"><span data-stu-id="eac9b-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="eac9b-108">SharePoint-sivuston käyttö oikeuksien mukauttaminen</span><span class="sxs-lookup"><span data-stu-id="eac9b-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="eac9b-109">Alikansion käyttö oikeuksien muuttaminen</span><span class="sxs-lookup"><span data-stu-id="eac9b-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="eac9b-110">Hallitsemattomien laitteiden käytön hallinta</span><span class="sxs-lookup"><span data-stu-id="eac9b-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="eac9b-111">SharePoint-tai yleinen-järjestelmänvalvojana voit estää tai rajoittaa SharePoint-ja OneDrive-sisällön käyttöä hallitsemattomista laitteista (ne, joita ei ole yhdistetty tai jotka on liitetty tai yhteensopiva Intunella).</span><span class="sxs-lookup"><span data-stu-id="eac9b-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="eac9b-112">**Verkko sijainnin rajoitus**</span><span class="sxs-lookup"><span data-stu-id="eac9b-112">**Network Location Restriction**</span></span>

<span data-ttu-id="eac9b-113">IT-järjestelmänvalvojana voit hallita SharePointin ja OneDriven resurssien käyttöä luotettavien verkko sijaintien perusteella.</span><span class="sxs-lookup"><span data-stu-id="eac9b-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="eac9b-114">Tätä kutsutaan myös sijaintiin perustuväksi käytännöksi.</span><span class="sxs-lookup"><span data-stu-id="eac9b-114">This is also known as location-based policy.</span></span> <span data-ttu-id="eac9b-115">Lisä tietoja on Ohje aiheessa [SharePoint Onlinen ja OneDrive-tietojen käytön hallinta verkko sijainnin perusteella](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="eac9b-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="eac9b-116">**Sivuston lukitus rajoitus**</span><span class="sxs-lookup"><span data-stu-id="eac9b-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="eac9b-117">SharePoint Onlinessa sinulla on mahdollisuus lukita sivustokokoelma, joten kukaan ei voi käyttää sitä.</span><span class="sxs-lookup"><span data-stu-id="eac9b-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="eac9b-118">Tämä määritetään PowerShellin ja [SharePoint Online-hallinta liittymän](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) kautta käyttämällä [joukkoa-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate-ominaisuutta.</span><span class="sxs-lookup"><span data-stu-id="eac9b-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="eac9b-119">**Sivuston tai alisivuston luomisen rajoittaminen käyttäjille**</span><span class="sxs-lookup"><span data-stu-id="eac9b-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="eac9b-120">Kun olet SharePoint-järjestelmänvalvoja tai yleinen järjestelmänvalvoja, voit antaa käyttäjien luoda ja hallita omia SharePoint-sivustojaan, määrittää, millaisia sivustot voivat luoda ja määrittää sivuston sijainnin.</span><span class="sxs-lookup"><span data-stu-id="eac9b-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="eac9b-121">Lisä tietoja on kohdassa [sivuston luomisen hallinta SharePoint Onlinessa](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="eac9b-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

