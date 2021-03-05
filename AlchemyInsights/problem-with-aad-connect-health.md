---
title: Ongelma AAD Connect Healthissa
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481466"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="79bb5-102">Ongelma AAD Connect Healthissa</span><span class="sxs-lookup"><span data-stu-id="79bb5-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="79bb5-103">Varmista, että sinulla on oikeus suorittaa toiminto.</span><span class="sxs-lookup"><span data-stu-id="79bb5-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="79bb5-104">Yleiset järjestelmänvalvojat voivat käyttää sitä oletusarvoisesti.</span><span class="sxs-lookup"><span data-stu-id="79bb5-104">Global Admins have access by default.</span></span> <span data-ttu-id="79bb5-105">Lisäksi roolipohjaisen käyttöoikeuksien [hallinnan avulla voit delegoida](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) rekisteröintioikeudet avustajalle.</span><span class="sxs-lookup"><span data-stu-id="79bb5-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="79bb5-106">Varmista, että tarvittavat päätepisteet ovat käytössä eikä niitä ole estetty palomuurin vuoksi.</span><span class="sxs-lookup"><span data-stu-id="79bb5-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="79bb5-107">Lisätietoja on [vaatimuksissa.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)</span><span class="sxs-lookup"><span data-stu-id="79bb5-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="79bb5-108">Rekisteröinti voi epäonnistua, koska verkkokerroksen kautta lähtevien yhteyksien SSL-tarkastus koskee.</span><span class="sxs-lookup"><span data-stu-id="79bb5-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="79bb5-109">Varmista, että olet vahvistanut Azure AD Connect Healthin ilmoitusasetukset.</span><span class="sxs-lookup"><span data-stu-id="79bb5-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="79bb5-110">Tarkista asetus.</span><span class="sxs-lookup"><span data-stu-id="79bb5-110">Please review your setting.</span></span> <span data-ttu-id="79bb5-111">Tämän [oppaan](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) avulla voit ymmärtää, miten voit määrittää Azure AD Connectin kuntoilmoitusten ilmoitusasetukset.</span><span class="sxs-lookup"><span data-stu-id="79bb5-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="79bb5-112">Lisätietoja AAD Connect Health -synkronointiraportista ja sen lataannista on objektitason [synkronointiraportissa.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="79bb5-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="79bb5-113">Jos haluat tehdä AAD Connect Health -ilmoitusten vianmäärityksen, katso [AAD Connect Healthin](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) tietojen tuoreusilmoituksia ja usein kysyttyjä kysymyksiä koskevat vianmääritysohjeet [AAD Connect Healthin asennusta varten.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="79bb5-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
