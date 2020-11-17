---
title: Ryhmän luominen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088690"
---
# <a name="create-a-group"></a><span data-ttu-id="ac26e-102">Ryhmän luominen</span><span class="sxs-lookup"><span data-stu-id="ac26e-102">Create a group</span></span>

<span data-ttu-id="ac26e-103">Tässä ohje aiheessa kerrotaan ryhmän luomisesta.</span><span class="sxs-lookup"><span data-stu-id="ac26e-103">This topic describes group creation.</span></span>

<span data-ttu-id="ac26e-104">**Ryhmän luomis oikeudet**</span><span class="sxs-lookup"><span data-stu-id="ac26e-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="ac26e-105">Varmista, että sinulla on oikeus luoda uusi ryhmä.</span><span class="sxs-lookup"><span data-stu-id="ac26e-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="ac26e-106">Yleiset järjestelmänvalvojat voivat poistaa ryhmän luomisen käytöstä Azure-portaalissa tai-paneelissa.</span><span class="sxs-lookup"><span data-stu-id="ac26e-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="ac26e-107">Sinun on ehkä luotava uusi ryhmä puolestasi tai annettava sinulle tarvittavat käyttö oikeudet.</span><span class="sxs-lookup"><span data-stu-id="ac26e-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="ac26e-108">**Ryhmän luomisen käyttö oikeuksien hallinta**</span><span class="sxs-lookup"><span data-stu-id="ac26e-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="ac26e-109">Yleiset järjestelmänvalvojat voivat hallita ryhmän luomis oikeuksia (turvallisuussyistä) tai Office 365-ryhmiä, jotka on luotu Azure-portaalissa tai-ohjaus paneelissa valitsemalla "käyttäjät voivat luoda käyttö oikeus ryhmiä Azure Portals-sovelluksessa" tai "käyttäjät voivat luoda Office 365-ryhmiä Azure Portals"-asetukset **kaikkien ryhmien**  >  **Yleiset-kohdassa (asetukset)**.</span><span class="sxs-lookup"><span data-stu-id="ac26e-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="ac26e-110">Voit myös rajoittaa ryhmän luontia ja valita käyttäjä ryhmän, jos käytössä on Azure Active Directory P1 Premium-käyttö oikeus.</span><span class="sxs-lookup"><span data-stu-id="ac26e-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="ac26e-111">**Tervetuloa-ilmoituksen poistaminen käytöstä uusissa Office 365-ryhmän jäsenille**</span><span class="sxs-lookup"><span data-stu-id="ac26e-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="ac26e-112">Office 365-ryhmiin lisätyille käyttäjille lähetetyt tervetuloilmoitukset voidaan poistaa käytöstä määrittämällä Määritä **yksilöllinen Groupwelcomemessage** -asetukseksi false PowerShellin avulla.</span><span class="sxs-lookup"><span data-stu-id="ac26e-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="ac26e-113">Lisä tietoja tästä asetuksesta on [täällä](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="ac26e-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

