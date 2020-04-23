---
title: Odottamaton monimenetelmäinen todentaminen
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: a664bd709062ec1335ebcf1f9adddc8aef917ac1
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766598"
---
# <a name="unexpected-multi-factor-authentication"></a><span data-ttu-id="d7539-102">Odottamaton monimenetelmäinen todentaminen</span><span class="sxs-lookup"><span data-stu-id="d7539-102">Unexpected multi-factor authentication</span></span>

<span data-ttu-id="d7539-103">Jos vuokraajasi luotiin 21.10.2019 jälkeen ja saat odottamattoman monimenetelmäistä todentamista koskevan kehotuksen, vuokraajassasi on luultavasti otettu käyttöön [oletusarvoiset suojausasetukset](https://aka.ms/securitydefaults).</span><span class="sxs-lookup"><span data-stu-id="d7539-103">If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span> 

<span data-ttu-id="d7539-104">Oletusarvoisten suojausasetusten hallinta:</span><span class="sxs-lookup"><span data-stu-id="d7539-104">To Manage security defaults:</span></span>

1. <span data-ttu-id="d7539-105">Kirjaudu [hallintakeskukseen](https://go.microsoft.com/fwlink/p/?linkid=834822) yleisen järjestelmänvalvojan tunnistetiedoilla.</span><span class="sxs-lookup"><span data-stu-id="d7539-105">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="d7539-106">Siirry kohtaan [Azure Active Directory -ominaisuudet](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="d7539-106">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="d7539-107">Napsauta sivun alareunassa **Hallitse oletusarvoisia suojausasetuksia**.</span><span class="sxs-lookup"><span data-stu-id="d7539-107">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="d7539-108">Napsauta **Kyllä** ottaaksesi suojauksen oletusasetukset käyttöön ja **Ei** poistaaksesi ne käytöstä.</span><span class="sxs-lookup"><span data-stu-id="d7539-108">Click **Yes** to enable security defaults and **No** to disable security defaults.</span></span>
