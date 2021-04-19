---
title: Ehdolliset käyttöoikeuskäytännöt
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
- "9002357"
- "4583"
ms.openlocfilehash: af95627d07d41add54f03c9254562b9be4e05d9b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817277"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="381e5-102">Ehdolliset käyttöoikeuskäytännöt</span><span class="sxs-lookup"><span data-stu-id="381e5-102">Conditional Access policies</span></span>

<span data-ttu-id="381e5-103">Ehdollinen käyttöoikeus on Azure AD:n ominaisuus, jonka avulla voit ottaa käyttöön ympäristösi sovellusten käyttöoikeuksia, jotka perustuvat tiettyihin ehtoihin ja joita hallitaan keskitetysti.</span><span class="sxs-lookup"><span data-stu-id="381e5-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="381e5-104">Lue lisätietoja [Azure AD:n ehdollisista käyttöoikeuksista](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="381e5-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="381e5-105">**Huomautus**: Jos vuokraajasi luotiin 21.10.2019 jälkeen ja saat odottamattoman monimenetelmäistä todentamista koskevan kehotuksen, vuokraajassasi on luultavasti otettu käyttöön [oletusarvoiset suojausasetukset](https://aka.ms/securitydefaults).</span><span class="sxs-lookup"><span data-stu-id="381e5-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="381e5-106">**Oletusarvoisten suojausasetusten hallinta**</span><span class="sxs-lookup"><span data-stu-id="381e5-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="381e5-107">Kirjaudu [hallintakeskukseen](https://go.microsoft.com/fwlink/p/?linkid=834822) yleisen järjestelmänvalvojan tunnistetiedoilla.</span><span class="sxs-lookup"><span data-stu-id="381e5-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="381e5-108">Siirry kohtaan [Azure Active Directory -ominaisuudet](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="381e5-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="381e5-109">Napsauta sivun alareunassa **Hallitse oletusarvoisia suojausasetuksia**.</span><span class="sxs-lookup"><span data-stu-id="381e5-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="381e5-110">Napsauta **Kyllä** ottaaksesi suojauksen oletusasetukset käyttöön tai **Ei** poistaaksesi ne käytöstä.</span><span class="sxs-lookup"><span data-stu-id="381e5-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>
