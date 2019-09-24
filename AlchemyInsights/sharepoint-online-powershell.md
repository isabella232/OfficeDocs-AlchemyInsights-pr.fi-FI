---
title: SharePoint Online PowerShell
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 00ec337ce34da9d3c3fba0a71602c3078a556552
ms.sourcegitcommit: 6b102e079a7d30298105fd811a67efb707d6d5bf
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/23/2019
ms.locfileid: "37122996"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="f1752-102">SharePoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="f1752-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="f1752-103">Työskentelen PowerShellin tai komento sarjojen kanssa SharePoint Onlinessa?</span><span class="sxs-lookup"><span data-stu-id="f1752-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="f1752-104">Lisä tietoja on alla olevissa linkeissä.</span><span class="sxs-lookup"><span data-stu-id="f1752-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="f1752-105">SharePointin online-hallinta liittymän käytön aloittaminen</span><span class="sxs-lookup"><span data-stu-id="f1752-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="f1752-106">Yhdistä SPO PowerShelliin monivaiheisen todennuksen avulla (MFA)</span><span class="sxs-lookup"><span data-stu-id="f1752-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="f1752-107">[SharePoint-mallit ja-käytännöt (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) sisältää PowerShell-komentojen kirjaston, jonka avulla voit suorittaa monimutkaisia hallinta toimia SPO: tä kohti.</span><span class="sxs-lookup"><span data-stu-id="f1752-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="f1752-108">Jos sinulla on ongelmia yhteyden muodostamisessa SPO-hallinta liittymään, varmista, että olet päivittänyt uusimpaan versioon ja yritä [tuoda moduuli uudelleen](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) käyttämällä *"Import-moduuli Microsoft. online. SharePoint. PowerShell"* -moduulia.</span><span class="sxs-lookup"><span data-stu-id="f1752-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="f1752-109">Jos yrität suorittaa asiakas puolen objekti mallin komento sarjoja, [SharePoint Online-asiakas komponenttien SDK](https://www.microsoft.com/download/details.aspx?id=42038) on asennettava paikalliseen tieto koneeseen.</span><span class="sxs-lookup"><span data-stu-id="f1752-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="f1752-110">Jos sinulla on ongelmia PowerShell-komento sarjojen suorittamisen kanssa, sinun kannattaa harkita PowerShellin suorittamista järjestelmänvalvojana ja [suoritus käytännön](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)muuttamista.</span><span class="sxs-lookup"><span data-stu-id="f1752-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>