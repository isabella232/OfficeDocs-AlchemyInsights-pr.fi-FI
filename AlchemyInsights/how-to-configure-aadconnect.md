---
title: 646 AADConnectin määrittäminen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722533"
---
# <a name="configure-sync-features"></a><span data-ttu-id="a8f8c-102">Synkronointiominaisuuksien määrittäminen</span><span class="sxs-lookup"><span data-stu-id="a8f8c-102">Configure sync features</span></span>

<span data-ttu-id="a8f8c-103">Azure AD Connect sisältää useita ominaisuuksia, jotka ovat oletusarvoisesti käytössä tai jotka voidaan ottaa käyttöön myöhemmin.</span><span class="sxs-lookup"><span data-stu-id="a8f8c-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="a8f8c-104">Jotkin ominaisuudet edellyttävät lisämäärityksiä tietyissä ympäristöissä.</span><span class="sxs-lookup"><span data-stu-id="a8f8c-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="a8f8c-105">[Suodatus](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) rajoittaa objektien synkronoinnin Azure AD:hen.</span><span class="sxs-lookup"><span data-stu-id="a8f8c-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="a8f8c-106">Oletusarvon mukaan kaikki käyttäjät, yhteystiedot, ryhmät ja Windows 10 -tietokonetilit synkronoidaan.</span><span class="sxs-lookup"><span data-stu-id="a8f8c-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="a8f8c-107">Voit sisällyttää tai jättää pois objekteja, jotka perustuvat toimialueisiin, oUs-kohteisiin tai muihin määritteisiin.</span><span class="sxs-lookup"><span data-stu-id="a8f8c-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="a8f8c-108">[Salasanan hajautussynkronointi](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synkronoi salasanan hajautusarvonsa paikallisesta Active Directorysta Azure AD:hen.</span><span class="sxs-lookup"><span data-stu-id="a8f8c-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="a8f8c-109">Tämä mahdollistaa salasanojen hallinnan yhdessä sijainnissa, mutta saman salasanan käyttäminen sekä paikallisissa että pilviympäristöissä.</span><span class="sxs-lookup"><span data-stu-id="a8f8c-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="a8f8c-110">Koska Active Directory on hallitseva lähde, voit käyttää omia salasanakäytäntöjäsi.</span><span class="sxs-lookup"><span data-stu-id="a8f8c-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="a8f8c-111">[Itsepalvelusalasanan nollauksen (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) avulla käyttäjät voivat nollata omat salasanansa pilvessä ja silti soveltaa paikallista salasanakäytäntöä.</span><span class="sxs-lookup"><span data-stu-id="a8f8c-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="a8f8c-112">[Laitteen takaisinkirjoitus](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) mahdollistaa azure AD:n rekisteröityjen laitteiden kirjoittamisen takaisin paikalliseen Active Directoryyn, jotta niitä voidaan käyttää ehdolliseen käyttöön.</span><span class="sxs-lookup"><span data-stu-id="a8f8c-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="a8f8c-113">[Estä vahingossa tapahtuvat poistot](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) on oletusarvoisesti käytössä, jotta vältettäisiin liian monta samanaikaista objektien poistoa (yli 500 objektia synkronointia kohden).</span><span class="sxs-lookup"><span data-stu-id="a8f8c-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="a8f8c-114">Voit muuttaa tätä asetusta organisaatiosi tarpeiden mukaan.</span><span class="sxs-lookup"><span data-stu-id="a8f8c-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="a8f8c-115">[Automaattinen päivitys](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) on oletusarvoisesti käytössä pika-asennuksissa, ja se auttaa varmistamaan, että Azure AD Connectin versio on aina ajan tasalla.</span><span class="sxs-lookup"><span data-stu-id="a8f8c-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
