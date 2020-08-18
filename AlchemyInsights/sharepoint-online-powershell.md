---
title: SharePoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 300c07e7f0010eae2bd4fe893ece9d09aab93ba5
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786886"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="a231d-102">SharePoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="a231d-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="a231d-103">Työskenteleminen PowerShellin tai komento sarjojen kanssa SharePoint Onlinessa?</span><span class="sxs-lookup"><span data-stu-id="a231d-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="a231d-104">Saat lisä tietoja alla olevista linkeistä.</span><span class="sxs-lookup"><span data-stu-id="a231d-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="a231d-105">SharePoint Online-hallinta liittymän käytön aloittaminen</span><span class="sxs-lookup"><span data-stu-id="a231d-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="a231d-106">Yhteyden muodostaminen SPO PowerShelliin multifactor-todennuksella (MFA)</span><span class="sxs-lookup"><span data-stu-id="a231d-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="a231d-107">[SharePoint-mallit ja-käytännöt (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) sisältää PowerShell-komentoja sisältävän kirjaston, jonka avulla voit suorittaa monimutkaisia hallinta toimia SPO:n hallintaan.</span><span class="sxs-lookup"><span data-stu-id="a231d-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="a231d-108">Jos sinulla on ongelmia SPO-hallinta liittymän kanssa, varmista, että olet päivittänyt uusimpaan versioon, ja yritä [tuoda moduuli uudelleen](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) *"Import-Module Microsoft. online. SharePoint. PowerShell"* -toiminnolla.</span><span class="sxs-lookup"><span data-stu-id="a231d-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="a231d-109">Jos yrität suorittaa asiakas puolen objekti malli komento sarjoja, sinulla on oltava [SharePoint Online client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) asennettuna paikalliseen tieto koneeseesi.</span><span class="sxs-lookup"><span data-stu-id="a231d-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="a231d-110">Jos sinulla on ongelmia komento sarjojen suorittamisessa PowerShellissä, kannattaa ehkä harkita PowerShellin suorittamista järjestelmänvalvojana ja [suoritus käytäntöjen](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)vaihtamista.</span><span class="sxs-lookup"><span data-stu-id="a231d-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>