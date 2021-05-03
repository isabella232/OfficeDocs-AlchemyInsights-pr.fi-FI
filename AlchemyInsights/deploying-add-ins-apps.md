---
title: Apu in käyttöönotto Microsoft 365 -sovellukset
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/30/2021
ms.locfileid: "52125202"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="96ca2-102">Apu in käyttöönotto Microsoft 365 -sovellukset</span><span class="sxs-lookup"><span data-stu-id="96ca2-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="96ca2-103">Keskitetty käyttöönotto on suositeltava tapa ottaa käyttöön Office ja ryhmiä organisaation käyttäjille ja ryhmille.</span><span class="sxs-lookup"><span data-stu-id="96ca2-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="96ca2-104">Ota apuohjelmat käyttöön noudattamalla seuraavia ohjeita:</span><span class="sxs-lookup"><span data-stu-id="96ca2-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="96ca2-105">**Huomautus:** Jos haluat asentaa apuohjelmat Office yksittäisenä käyttäjänä, katso Lisätietoja apuohjelmien tarkasteleminen, hallinta [ja asentaminen Office ohjelmissa.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="96ca2-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="96ca2-106">Varmista myös, että Office Storen apuohjelmat on otettu käyttöön.</span><span class="sxs-lookup"><span data-stu-id="96ca2-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> 

1. <span data-ttu-id="96ca2-107">Varmista, että ympäristösi täyttää apuohjelmat käyttöönoton vaatimukset keskitetyn käyttöönoton avulla.</span><span class="sxs-lookup"><span data-stu-id="96ca2-107">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="96ca2-108">Lisätietoja on kohdassa [Vaatimukset](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span><span class="sxs-lookup"><span data-stu-id="96ca2-108">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="96ca2-109">Siirry **Asetukset**  >  **apusovellusten**  >  **käyttöönottoon** Microsoft 365 hallintakeskuksessa.</span><span class="sxs-lookup"><span data-stu-id="96ca2-109">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="96ca2-110">Huomautukset:</span><span class="sxs-lookup"><span data-stu-id="96ca2-110">Notes:</span></span> 

- <span data-ttu-id="96ca2-111">Integroidut sovellukset edellyttävät, että järjestelmänvalvojalla on yleisen järjestelmänvalvojan Exchange järjestelmänvalvojan oikeudet.</span><span class="sxs-lookup"><span data-stu-id="96ca2-111">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="96ca2-112">Kun apuohjelmat otetaan käyttöön useille käyttäjille, on suositeltavaa tehdä tehtäviä käyttämällä ryhmiä yksittäisten käyttäjien sijaan.</span><span class="sxs-lookup"><span data-stu-id="96ca2-112">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="96ca2-113">Lisätietoja on kohdassa Huomioon [otettavia seikkoja, kun apuohjelma määritetään käyttäjille ja ryhmille.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)</span><span class="sxs-lookup"><span data-stu-id="96ca2-113">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="96ca2-114">Keskitetty käyttöönotto ei tue sisäkkäisten ryhmien tai pääryhmien käyttäjiä.</span><span class="sxs-lookup"><span data-stu-id="96ca2-114">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="96ca2-115">Lisätietoja on kohdassa [Käyttäjä- ja ryhmämääritykset.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)</span><span class="sxs-lookup"><span data-stu-id="96ca2-115">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="96ca2-116">Varmista, että Microsoft 365 app management service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') on otettu käyttöön käyttäjille.</span><span class="sxs-lookup"><span data-stu-id="96ca2-116">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="96ca2-117">Lisätietoja on kohdassa [Sovelluksen ominaisuuksien määrittäminen.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)</span><span class="sxs-lookup"><span data-stu-id="96ca2-117">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="96ca2-118">Jos sinulla on ongelmia apuohjelmien käyttöönotossa integroitujen sovellusten avulla, kokeile käyttöönottoa [apuohjelmilla.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)</span><span class="sxs-lookup"><span data-stu-id="96ca2-118">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="96ca2-119">Lisätietoja on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="96ca2-119">For more information, see:</span></span>

<span data-ttu-id="96ca2-120">[Apu in käyttöönotto hallintakeskuksessa](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Apu in hallintakeskuksessa](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Aputyökalujen hallinta keskitetyn käyttöönoton PowerShell-cmdlet-komentojen avulla](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Julkaise Office käyttämällä keskitettyä käyttöönottoa Microsoft 365 hallintakeskuksessa](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Vianmääritys: Käyttäjät eivät näe apu ins.](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Käyttäjävirheiden Office apuohjelmat](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="96ca2-120">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>