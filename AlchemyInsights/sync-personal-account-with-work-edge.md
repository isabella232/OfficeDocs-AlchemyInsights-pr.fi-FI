---
title: Henkilökohtaisen tilin ja työtilin synkronoinnin salliminen Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9127"
- "9004429"
ms.openlocfilehash: da435b37b689e97ca51ce5cf94eb7e7d71eb972060526989239310fac1460628
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813394"
---
# <a name="enable-a-user-to-sync-a-personal-account-with-the-work-account-in-microsoft-edge"></a>Henkilökohtaisen tilin ja työtilin synkronoinnin salliminen Microsoft Edge

Varmista, että täytät seuraavat ehdot:

- Yrityksen tilavierailu otetaan käyttöön Azure Active Directory hallintakeskuksessa, joka edellyttää Azure Active Directory Premium tai Enterprise Mobility + Security (EMS). Lisätietoja on kohdassa Enterprise [State Roamingin ottaminen käyttöön Azure Active Directory.](/azure/active-directory/devices/enterprise-state-roaming-enable)
- Toinen tai molemmat seuraavista ehdoista täyttyy:
    - Azure Information Protection -palvelu on otettu käyttöön vuokraajassa. Lisätietoja on kohdassa [Azure Rights Management Protectionin aktivoiminen Microsoft 365 -hallintakeskus.](/azure/information-protection/activate-office365)
    - Kaikkien Azure Active Directory tai vuokraajalle on otettu käyttöön Azure Active Directory (ENTERPRISE State Roaming) -ominaisuus. Lisätietoja on kohdassa Mikä [on yrityksen verkkovierailu?](/azure/active-directory/devices/enterprise-state-roaming-overview).

Jos AIP jaSÄHKÖPOSTIVIESTI on molemmat poistettu käytöstä, virhesanoma ilmoittaa käyttäjille, että synkronointi ei ole käytettävissä tileinsä yhteydessä.
