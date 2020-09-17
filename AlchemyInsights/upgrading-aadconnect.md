---
title: 932 päivitys AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806036"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="570c4-102">Azure AD Connect-päivitys</span><span class="sxs-lookup"><span data-stu-id="570c4-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="570c4-103">Oletusarvoisesti automaattinen päivitys on käytössä Azure AD Connectin avulla, mikä auttaa varmistamaan, että käytössäsi on uusin versio.</span><span class="sxs-lookup"><span data-stu-id="570c4-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="570c4-104">Voit tarkistaa automaattiset päivitys asetukset käyttämällä **Get-ADSyncAutoUpgrade-cmdlet-** komennolla Azure AD PowerShellissä.</span><span class="sxs-lookup"><span data-stu-id="570c4-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="570c4-105">Cmdlet-komento palauttaa jonkin seuraavista arvoista:</span><span class="sxs-lookup"><span data-stu-id="570c4-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="570c4-106">**Käytössä**: Automaattinen päivitys on käytössä.</span><span class="sxs-lookup"><span data-stu-id="570c4-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="570c4-107">Ei **käytössä**: Automaattinen päivitys on poistettu käytöstä.</span><span class="sxs-lookup"><span data-stu-id="570c4-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="570c4-108">**Keskeytys**: järjestelmä ei ole enää oikeutettu automaattisten päivitysten vastaanottoon.</span><span class="sxs-lookup"><span data-stu-id="570c4-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="570c4-109">Et voi määrittää tätä arvoa. järjestelmä on asettanut sen.</span><span class="sxs-lookup"><span data-stu-id="570c4-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="570c4-110">Lisä tietoja on kohdassa [Automaattinen päivitys](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="570c4-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="570c4-111">Jos haluat ladata uusimman Azure AD Connect-version, siirry [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="570c4-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
