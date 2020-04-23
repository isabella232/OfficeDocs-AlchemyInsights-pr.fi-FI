---
title: 932 AADConnectin päivittäminen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: fcc5fddb5cfd15407d0533449035317d187931ed
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766490"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="c2986-102">Azure AD Connectin päivittäminen</span><span class="sxs-lookup"><span data-stu-id="c2986-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="c2986-103">Oletusarvon mukaan automaattinen päivitys on käytössä Azure AD Connectissa, mikä auttaa varmistamaan, että käytössäsi on uusin versio.</span><span class="sxs-lookup"><span data-stu-id="c2986-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="c2986-104">Voit tarkistaa automaattiset päivitysasetukset Azure AD PowerShellin **Get-ADSyncAutoUpgrade-cmdlet-komentoa** käyttämällä.</span><span class="sxs-lookup"><span data-stu-id="c2986-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="c2986-105">Cmdlet palauttaa jonkin seuraavista arvoista:</span><span class="sxs-lookup"><span data-stu-id="c2986-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="c2986-106">**Käytössä:** Automaattinen päivitys on käytössä.</span><span class="sxs-lookup"><span data-stu-id="c2986-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="c2986-107">**Ei käytössä**: Automaattinen päivitys on poistettu käytöstä.</span><span class="sxs-lookup"><span data-stu-id="c2986-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="c2986-108">**Keskeytetty:** Järjestelmä ei ole enää oikeutettu vastaanottamaan automaattisia päivityksiä.</span><span class="sxs-lookup"><span data-stu-id="c2986-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="c2986-109">Tätä arvoa ei voi määrittää. Se on asetettu järjestelmä.</span><span class="sxs-lookup"><span data-stu-id="c2986-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="c2986-110">Lisätietoja on kohdassa [Automaattinen päivitys](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="c2986-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="c2986-111">Jos haluat ladata Azure AD Connectin [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)uusimman version, siirry kohtaan .</span><span class="sxs-lookup"><span data-stu-id="c2986-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
