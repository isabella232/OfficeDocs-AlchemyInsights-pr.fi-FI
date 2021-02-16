---
title: Laitteen takaisin kirjoittaminen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "8279"
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256750"
---
# <a name="device-writeback"></a><span data-ttu-id="5a9da-102">Laitteen takaisin kirjoittaminen</span><span class="sxs-lookup"><span data-stu-id="5a9da-102">Device Writeback</span></span>

<span data-ttu-id="5a9da-103">Laitteen takaisinkirjoitusta käytetään seuraavissa tilanteissa:</span><span class="sxs-lookup"><span data-stu-id="5a9da-103">Device Writeback is used in the following scenarios:</span></span>

- <span data-ttu-id="5a9da-104">[Windows Hello for Businessin käyttöönotto yhdistelmävarmenteen luottamusympäristön avulla](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span><span class="sxs-lookup"><span data-stu-id="5a9da-104">Enable [Windows Hello for Business using hybrid certificate trust deployment](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span></span>
- <span data-ttu-id="5a9da-105">Ehdollisen käyttöoikeuden ottaminen käyttöön ADFS (2012 R2 tai uudempi) -suojattujen sovellusten (jotka perustuvat osapuolen luottamuksiin) perusteella</span><span class="sxs-lookup"><span data-stu-id="5a9da-105">Enable Conditional Access based on devices to ADFS (2012 R2 or higher) protected applications (relying party trusts)</span></span>

    > [!NOTE]
    > <span data-ttu-id="5a9da-106">Laitteen takaisin kirjoittaminen edellyttää Azure AD Premium -tilausta.</span><span class="sxs-lookup"><span data-stu-id="5a9da-106">A subscription to Azure AD Premium is required for device writeback.</span></span>

<span data-ttu-id="5a9da-107">Tämä antaa lisäturvaa ja varmuuden siitä, että sovellusten käyttöoikeus myönnetään vain luotettuihin laitteisiin.</span><span class="sxs-lookup"><span data-stu-id="5a9da-107">This provides additional security and assurance that access to applications is granted only to trusted devices.</span></span> <span data-ttu-id="5a9da-108">Lisätietoja ehdollisesta käyttöoikeuksien [](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) käyttämisestä on kohdassa Riskien hallinta ehdollisella käyttöomme ja paikallisen ehdollisen käyttöoikeuden määrittäminen [Azure Active Directory -laiterekisteröinnin avulla.](https://docs.microsoft.com/azure/active-directory/devices/overview)</span><span class="sxs-lookup"><span data-stu-id="5a9da-108">For more information on Conditional Access, see [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) and [Setting up On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).</span></span>

<span data-ttu-id="5a9da-109">Lisätietoja laitteen takaisin kirjoittamisen ottamalla käyttöön laitteissa on kohdassa [Ota laitteen takaisin kirjoittaminen takaisin käyttöön.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)</span><span class="sxs-lookup"><span data-stu-id="5a9da-109">For more information on Enabling Device Writeback for Devices, see [Enable Device Writeback](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).</span></span>
