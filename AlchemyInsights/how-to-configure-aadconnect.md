---
title: 646 AADConnect-asetusten määrittäminen
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
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704486"
---
# <a name="configure-sync-features"></a><span data-ttu-id="5c203-102">Synkronointi ominaisuuksien määrittäminen</span><span class="sxs-lookup"><span data-stu-id="5c203-102">Configure sync features</span></span>

<span data-ttu-id="5c203-103">Azure AD Connect sisältää useita ominaisuuksia, jotka ovat oletusarvoisesti käytössä tai jotka voit ottaa käyttöön myöhemmin.</span><span class="sxs-lookup"><span data-stu-id="5c203-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="5c203-104">Jotkin ominaisuudet vaativat lisä määrityksiä tietyissä ympäristöissä.</span><span class="sxs-lookup"><span data-stu-id="5c203-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="5c203-105">[Suodattaminen](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) rajoittaa objektien synkronoinnin Azure AD:hen.</span><span class="sxs-lookup"><span data-stu-id="5c203-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="5c203-106">Oletusarvoisesti kaikki käyttäjät, yhteys tiedot, ryhmät ja Windows 10-tieto kone tunnukset synkronoidaan.</span><span class="sxs-lookup"><span data-stu-id="5c203-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="5c203-107">Voit sisällyttää tai jättää pois objekteja toimi alueiden, organisaatio yksiköiden tai muiden määritteiden perusteella.</span><span class="sxs-lookup"><span data-stu-id="5c203-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="5c203-108">[Salasana hajautus synkronointi](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) Synkronoi Sala sanan hajautus arvon paikallisesta Active Directorysta Azure AD:hen.</span><span class="sxs-lookup"><span data-stu-id="5c203-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="5c203-109">Tämä mahdollistaa Sala sanojen hallinnan yhdessä sijainnissa, mutta käyttää samaa Sala sanaa sekä paikallisessa että pilvi ympäristössä.</span><span class="sxs-lookup"><span data-stu-id="5c203-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="5c203-110">Koska Active Directory on määräävä lähde, voit käyttää omaa salasana käytäntöä.</span><span class="sxs-lookup"><span data-stu-id="5c203-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="5c203-111">[Omatoiminen Sala sanan palautus (sspr)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) mahdollistaa sen, että käyttäjät voivat vaihtaa Sala sanansa pilvi palvelussa, mutta silti ottaa käyttöön paikallisen salasana käytäntönsä.</span><span class="sxs-lookup"><span data-stu-id="5c203-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="5c203-112">[Laitteen takaisinkirjoitus](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) mahdollistaa sen, että Azure AD:ssä rekisteröityneet laitteet voidaan kirjoittaa takaisin paikalliseen Active Directoryyn, jotta niitä voidaan käyttää ehdollisen käytön aikana.</span><span class="sxs-lookup"><span data-stu-id="5c203-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="5c203-113">[Estä tahattomat poistot](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) ovat oletusarvoisesti käytössä, jotta estetään liian monta samanaikaista objektien poistoa (yli 500 objektia synkronoinnin aikana).</span><span class="sxs-lookup"><span data-stu-id="5c203-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="5c203-114">Voit muuttaa tätä asetusta vastaamaan organisaatiosi tarpeita.</span><span class="sxs-lookup"><span data-stu-id="5c203-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="5c203-115">[Automaattinen päivitys](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) on oletusarvoisesti käytössä pikaasennuksissa ja auttaa varmistamaan, että Azure AD Connect-versiosi on aina ajan tasalla.</span><span class="sxs-lookup"><span data-stu-id="5c203-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
