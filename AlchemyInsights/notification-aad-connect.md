---
title: Ilmoitus AAD Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035429"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="ca717-102">Ilmoitus AAD Connectista</span><span class="sxs-lookup"><span data-stu-id="ca717-102">Notification AAD Connect</span></span>

- <span data-ttu-id="ca717-103">Varmista, että sinulla on oikeus suorittaa toiminto.</span><span class="sxs-lookup"><span data-stu-id="ca717-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="ca717-104">Yleiset järjestelmänvalvojat voivat käyttää sitä oletusarvoisesti.</span><span class="sxs-lookup"><span data-stu-id="ca717-104">Global Admins have access by default.</span></span> <span data-ttu-id="ca717-105">Lisäksi roolipohjaisen käyttöoikeuksien [hallinnan avulla voit delegoida](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) rekisteröintioikeudet avustajalle.</span><span class="sxs-lookup"><span data-stu-id="ca717-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="ca717-106">Varmista, että tarvittavat päätepisteet ovat käytössä eikä niitä ole estetty palomuurin vuoksi.</span><span class="sxs-lookup"><span data-stu-id="ca717-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="ca717-107">Lisätietoja on [vaatimuksissa.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)</span><span class="sxs-lookup"><span data-stu-id="ca717-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="ca717-108">Rekisteröinti voi epäonnistua, koska verkkokerroksen kautta lähtevien yhteyksien SSL-tarkastus koskee.</span><span class="sxs-lookup"><span data-stu-id="ca717-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="ca717-109">Varmista, että olet vahvistanut Azure AD Connect Healthin ilmoitusasetukset ja tarkista asetukset.</span><span class="sxs-lookup"><span data-stu-id="ca717-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="ca717-110">Lisätietoja Azure AD Connect Health -ilmoitusten ilmoitusasetusten määrittämisestä on tässä [oppaassa.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)</span><span class="sxs-lookup"><span data-stu-id="ca717-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="ca717-111">Lisätietoja AAD Connect Health -synkronointiraportista ja sen lataannista on objektitason [synkronointiraportissa.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="ca717-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="ca717-112">AAD Connect Health -ilmoitusten vianmäärityksessä on [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) -tietojen tuoreusilmoituksia ja usein kysyttyjä kysymyksiä koskevat vianmääritysohjeet yleisistä [AAD Connect Health -asennuskysymyksistä.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="ca717-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
