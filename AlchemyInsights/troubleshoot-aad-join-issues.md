---
title: Azure AD:n liittymisongelmien vianmääritys
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404632"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Azure AD:n liittymisongelmien vianmääritys

1. Jos määrität laiterekisteröintiä ensimmäistä kertaa, varmista, että olet tutustunut [Azure Active Directoryn](https://docs.microsoft.com/azure/active-directory/devices/overview) laitehallinnan esittelyyn, joka opastaa sinua, miten saat hallitut laitteet Azure AD:lle. 
1. Jos rekisteröit laitteita suoraan Azure AD:lle ja rekisteröit ne Intuneen, sinun on varmistettava, että olet määrittänyt [Intunen](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) ja että käyttöoikeudet ovat käytössä ensin. [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign)
1. Varmista, että sinulla on oikeus suorittaa toimintoja Azure AD:ssä. Vain Azure AD:n yleinen järjestelmänvalvoja voi hallita laiterekisteröinnin asetuksia.
1. Azure AD :n liittymisen käyttöönotto on ohjeaiheessa [Azure AD -liitoksen suunnittelu.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)

Lisätietoja Azure AD -liittymisen yleisimpiä ongelmia ratkaisemisesta on [Azure Ad Joinin](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) usein kysytyissä kysymyksissä ja Windows 10 Pro -laitteessa on kohdassa [Windows 10 Pro -koneeseen](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) liittyminen Azure AD:lle ei onnistu - Päivitys on tarpeen – Microsoft Community
