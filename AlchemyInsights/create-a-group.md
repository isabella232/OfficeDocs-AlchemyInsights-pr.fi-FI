---
title: Ryhmän luominen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816345"
---
# <a name="create-a-group"></a><span data-ttu-id="cef70-102">Ryhmän luominen</span><span class="sxs-lookup"><span data-stu-id="cef70-102">Create a group</span></span>

<span data-ttu-id="cef70-103">Tässä ohjeaiheessa kerrotaan ryhmien luomisesta.</span><span class="sxs-lookup"><span data-stu-id="cef70-103">This topic describes group creation.</span></span>

<span data-ttu-id="cef70-104">**Ryhmän luontioikeus**</span><span class="sxs-lookup"><span data-stu-id="cef70-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="cef70-105">Varmista, että sinulla on oikeus luoda uusi ryhmä.</span><span class="sxs-lookup"><span data-stu-id="cef70-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="cef70-106">Yleiset järjestelmänvalvojat voivat poistaa käytöstä ryhmien luomisen Azure-portaalissa tai käyttöpaneelissa.</span><span class="sxs-lookup"><span data-stu-id="cef70-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="cef70-107">Tarvitset ehkä järjestelmänvalvojan, jotta voit luoda uuden ryhmän, tai antaa sinulle tarvittavat käyttöoikeudet.</span><span class="sxs-lookup"><span data-stu-id="cef70-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="cef70-108">**Ryhmän luontioikeuksien hallinta**</span><span class="sxs-lookup"><span data-stu-id="cef70-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="cef70-109">Yleiset järjestelmänvalvojat voivat hallita ryhmien luontioikeuksia (tietoturvasyistä) tai Azure-portaalissa tai -paneelissa luotuja Office 365 -ryhmiä valitsemalla Käyttäjät voivat luoda käyttöoikeusryhmiä Azure-portaaleissa tai Käyttäjät voivat luoda Office 365 -ryhmiä Azure-portaaleissa -vaihtoehdot Kaikki ryhmät Yleiset   >  **(Asetukset)**-kohdassa.</span><span class="sxs-lookup"><span data-stu-id="cef70-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="cef70-110">Voit myös rajoittaa ryhmien luomisen valitsemaan käyttäjäryhmän, jos sinulla on Azure Active Directory P1 Premium -käyttöoikeus.</span><span class="sxs-lookup"><span data-stu-id="cef70-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="cef70-111">**Tervetuloilmoituksen poistaminen käytöstä uusille Office 365 -ryhmän jäsenille**</span><span class="sxs-lookup"><span data-stu-id="cef70-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="cef70-112">Office 365 -ryhmiin lisätyille käyttäjille lähetettävä tervetuloilmoitus voidaan poistaa käytöstä määrittämällä **UnifiedGroupWelcomeMessageEnabled-arvoksi** Epätosi Powershellissä.</span><span class="sxs-lookup"><span data-stu-id="cef70-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="cef70-113">Lisätietoja tästä [asetuksesta on täällä](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="cef70-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

