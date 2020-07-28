---
title: Teamsin yksityisen kanavan poistaminen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439328"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="a4ab9-102">Teamsin yksityisen kanavan poistaminen</span><span class="sxs-lookup"><span data-stu-id="a4ab9-102">Delete a Teams private channel</span></span>

<span data-ttu-id="a4ab9-103">Microsoft on tietoinen ryhmäsiekoisen yksityisen kanavan poistamisesta, jos sharepoint-säilytyskäytännöt ovat käytössä taustalla olevassa SharePoint-sivustossa.</span><span class="sxs-lookup"><span data-stu-id="a4ab9-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="a4ab9-104">Microsoft työstää korjausta.</span><span class="sxs-lookup"><span data-stu-id="a4ab9-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="a4ab9-105">Sillä välin voit poistaa yksityisen kanavan seuraavien kiertotapojen avulla.</span><span class="sxs-lookup"><span data-stu-id="a4ab9-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="a4ab9-106">**Jätä ryhmä/sivustokokoelma pois Sharepoint-säilytyskäytännöstä.**</span><span class="sxs-lookup"><span data-stu-id="a4ab9-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="a4ab9-107">Siirry Office 365 -hallintaportaaliin ja valitse vasemmasta siirtymisruudusta **Näytä kaikki.**</span><span class="sxs-lookup"><span data-stu-id="a4ab9-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="a4ab9-108">Siirry **Hallintakeskukset -kohdassa** **Suojaus &**  >  **Yhteensopivuustietojen menetyksen estokäytäntö**  >  **Policy**.</span><span class="sxs-lookup"><span data-stu-id="a4ab9-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="a4ab9-109">Määritä Sharepoint-sivustoihin liittyvät käytännöt ja muokkaa käytäntöä niin, että yksityisen kanavan sisältävän ryhmän Sharepoint-sivustoa EI sisällytetä säilytyskäytäntöön.</span><span class="sxs-lookup"><span data-stu-id="a4ab9-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="a4ab9-110">Tallenna käytäntö.</span><span class="sxs-lookup"><span data-stu-id="a4ab9-110">Save the policy.</span></span>
    <span data-ttu-id="a4ab9-111">Käytäntöasetusten voimaantulo voi kestää jopa 24 tuntia.</span><span class="sxs-lookup"><span data-stu-id="a4ab9-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="a4ab9-112">Kun sivusto on poistettu, voit poistaa yksityisen kanavan.</span><span class="sxs-lookup"><span data-stu-id="a4ab9-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="a4ab9-113">Voit ***ehkä*** poistaa yksityisen kanavan Käyttämällä Microsoft Teamia Android-laitteessasi.</span><span class="sxs-lookup"><span data-stu-id="a4ab9-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="a4ab9-114">Lisätietoja SharePointista [on ohjeaiheessa SharePoint Onlinen tai OneDrive for Businessin kohteiden poistaminen](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold)ei onnistu .</span><span class="sxs-lookup"><span data-stu-id="a4ab9-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>