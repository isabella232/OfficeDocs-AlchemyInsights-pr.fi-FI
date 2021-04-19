---
title: SharePoint- tai OneDrive-hallintakeskusta ei voi käyttää
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: 7ba4a9c6995c03dd21e0e1aa387e407d41a08fb1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824432"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a><span data-ttu-id="3f90a-102">SharePoint- tai OneDrive-hallintakeskusta ei voi käyttää</span><span class="sxs-lookup"><span data-stu-id="3f90a-102">Unable to access SharePoint or OneDrive admin center</span></span>

- <span data-ttu-id="3f90a-103">Jos SharePoint- tai OneDrive-hallintakeskussivustosi ei ole käytettävissä tai se ei ole käytettävissä, voi olla tilapäinen palveluongelma, jossa käyttäjillä voi olla ajoittaisia viiveitä tai siirtymisvirheitä SharePoint-sivustojen tai OneDrive-sisällön käytön aikana.</span><span class="sxs-lookup"><span data-stu-id="3f90a-103">If your SharePoint or OneDrive Admin center site is inaccessible or unavailable, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="3f90a-104">Tarkista Palvelun [kunto -koontinäytöstä,](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) vaikuttaako se organisaatioosi.</span><span class="sxs-lookup"><span data-stu-id="3f90a-104">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

- <span data-ttu-id="3f90a-105">Yleisille ja SharePoint-järjestelmänvalvojille on oltava määritetty SharePoint-käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="3f90a-105">Global and SharePoint admins need to be assigned a SharePoint license.</span></span> <span data-ttu-id="3f90a-106">Juuri luoduilla tileillä, jotka on juuri määritetty SharePoint-käyttöoikeus- tai järjestelmänvalvojan roolilla, voi i ie iä sharePointia käyttää, kuten "käyttö estetty" tai "käyttäjää ei löydy".</span><span class="sxs-lookup"><span data-stu-id="3f90a-106">Newly created accounts just assigned with a SharePoint License or Admin role might experience issues accessing SharePoint, like "access denied" or "user not found."</span></span> <span data-ttu-id="3f90a-107">Anna vähintään 24 tuntia aikaa suorittaa synkronointi eri järjestelmissä.</span><span class="sxs-lookup"><span data-stu-id="3f90a-107">Please give at least 24 hours for sync to complete across our systems.</span></span> <span data-ttu-id="3f90a-108">Ymmärrämme, että 24 tuntia voi vaikuttaa pitkältä ajasta.</span><span class="sxs-lookup"><span data-stu-id="3f90a-108">We understand that 24 hours may seem like a long time.</span></span> <span data-ttu-id="3f90a-109">Monissa tapauksissa ongelmaan on jo tehty ratkaisu.</span><span class="sxs-lookup"><span data-stu-id="3f90a-109">In many cases, we're already working on a solution.</span></span>

- <span data-ttu-id="3f90a-110">Privileged Identity Management[(PIM)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)-käyttäjät voivat saada käyttö estettyjä tietoja, jos käyttöaikaikkuna on hyvin pieni, katso [Pim-tilien käyttö estetty.](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="3f90a-110">Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new))  users may receive access denied if allowed access time window is very small, see  [Access denied to PIM accounts](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).</span></span>