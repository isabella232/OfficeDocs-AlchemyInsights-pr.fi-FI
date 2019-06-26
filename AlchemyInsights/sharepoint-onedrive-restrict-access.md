---
title: Kirjoita SharePoint- tai OneDrive käytön rajoittaminen
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: db84f77208dca60c6dee98cdb0c7f1ea7fa8fe17
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223709"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="79647-102">Kirjoita SharePoint- tai OneDrive käytön rajoittaminen</span><span class="sxs-lookup"><span data-stu-id="79647-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="79647-103">SharePoint Online/OneDrive palvelujen käytön rajoittaminen monilla tavoilla.</span><span class="sxs-lookup"><span data-stu-id="79647-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="79647-104">Seuraavassa esitetyt menetelmät eri access-rajoitus.</span><span class="sxs-lookup"><span data-stu-id="79647-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="79647-105">**Käyttöoikeuden rajoittaminen**</span><span class="sxs-lookup"><span data-stu-id="79647-105">**Permission Restriction**</span></span>

<span data-ttu-id="79647-106">SharePoint Online-ja liiketoiminnan OneDrive olemme rajoittaa esimerkiksi sivustot, tiedostot ja kansiot vain myöntäminen ryhmiä ja vastaavien käyttäjien olisi päästävä.</span><span class="sxs-lookup"><span data-stu-id="79647-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="79647-107">Voit mukauttaa SharePoint-luettelon tai kirjaston käyttöoikeudet</span><span class="sxs-lookup"><span data-stu-id="79647-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="79647-108">Voit mukauttaa SharePoint-sivuston käyttöoikeudet</span><span class="sxs-lookup"><span data-stu-id="79647-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="79647-109">Muuta alikansion käyttöoikeuksia</span><span class="sxs-lookup"><span data-stu-id="79647-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="79647-110">Hallitsemattomien laitteiden käytön hallinta</span><span class="sxs-lookup"><span data-stu-id="79647-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="79647-111">SharePoint-tai Office 365: ssä yleisen järjestelmänvalvojan estää tai rajoittaa pääsyä laitteiden hallitsemattomaan SharePoint-ja OneDrive (nämä hybridi liitettyjen tai yhteensopiva Intune AD).</span><span class="sxs-lookup"><span data-stu-id="79647-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="79647-112">**Verkon sijainti rajoittamiseen**</span><span class="sxs-lookup"><span data-stu-id="79647-112">**Network Location Restriction**</span></span>

<span data-ttu-id="79647-113">IT-järjestelmänvalvojana voit hallita SharePoint- ja OneDrive määriteltyjen verkkosijainteihin, joihin luotat perustuvat resurssien käyttöä.</span><span class="sxs-lookup"><span data-stu-id="79647-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="79647-114">Tätä kutsutaan myös sijaintiin perustuva käytäntö.</span><span class="sxs-lookup"><span data-stu-id="79647-114">This is also known as location-based policy.</span></span> <span data-ttu-id="79647-115">Lisätietoja on ohjeaiheessa [SharePoint Online ja OneDrive verkkosijaintiin perustuvien tietojen käytön valvonta](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="79647-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="79647-116">**Sivustorajoitusta lukitus**</span><span class="sxs-lookup"><span data-stu-id="79647-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="79647-117">Sinulla on mahdollisuus lukita niin, että kukaan pääsee sivustokokoelman sisällä SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="79647-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="79647-118">Määritä PowerShell- ja [SharePoint Online-hallintaliittymä](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) käyttämällä [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState-ominaisuuden kautta.</span><span class="sxs-lookup"><span data-stu-id="79647-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="79647-119">**Sivustojen ja alisivustojen luominen estäminen**</span><span class="sxs-lookup"><span data-stu-id="79647-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="79647-120">SharePoint-järjestelmänvalvoja tai yleisen järjestelmänvalvojan Office 365: ssä, voit antaa käyttäjien luoda ja hallinnoida omia SharePoint-sivustot, selvittää, mitä sivustoja he voivat luoda, ja määritä sijainti sivustot.</span><span class="sxs-lookup"><span data-stu-id="79647-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="79647-121">Lisätietoja on kohdassa [Hallitse sivuston luominen SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="79647-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

