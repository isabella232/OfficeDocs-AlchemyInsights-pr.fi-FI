---
title: Sharepoint Online -PowerShell
ms.author: v-todmc
author: todmccoy
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
ms.openlocfilehash: 8c270748fc75f929371fbb2856daad3ae61a1540
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764258"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="4e593-102">Sharepoint Online -PowerShell</span><span class="sxs-lookup"><span data-stu-id="4e593-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="4e593-103">PowerShellin tai Komentosarjojen käyttäminen Sharepoint Onlinessa?</span><span class="sxs-lookup"><span data-stu-id="4e593-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="4e593-104">Lisätietoja on alla olevissa linkeissä.</span><span class="sxs-lookup"><span data-stu-id="4e593-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="4e593-105">SharePoint Online -hallintaliittymän käytön aloittaminen</span><span class="sxs-lookup"><span data-stu-id="4e593-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="4e593-106">Yhteyden muodostaminen SPO PowerShelliin monitekijätodennuksen (MFA) avulla</span><span class="sxs-lookup"><span data-stu-id="4e593-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="4e593-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) sisältää PowerShell-komentojen kirjaston, jonka avulla voit suorittaa monimutkaisia hallintatoimintoja spo:ta kohtaan.</span><span class="sxs-lookup"><span data-stu-id="4e593-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="4e593-108">Jos sinulla on ongelmia yhteyden muodostamisessa SPO:n hallintaliittymän kanssa, varmista, että olet päivittänyt uusimpaan versioon, ja yritä [tuoda moduuli uudelleen](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) *"Import-Module Microsoft.Online.SharePoint.PowerShell" -toiminnon avulla.*</span><span class="sxs-lookup"><span data-stu-id="4e593-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="4e593-109">Jos yrität suorittaa asiakaspuolen objektimallikomentosarjoja, [sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) on oltava asennettuna paikalliseen tietokoneeseen.</span><span class="sxs-lookup"><span data-stu-id="4e593-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="4e593-110">Jos sinulla on ongelmia komentosarjojen suorittamisessa PowerShellistä, kannattaa harkita PowerShellin suorittamista järjestelmänvalvojana ja [suorituskäytännön](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)muuttamista.</span><span class="sxs-lookup"><span data-stu-id="4e593-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>