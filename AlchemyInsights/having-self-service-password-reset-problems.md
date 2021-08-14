---
title: Onko omatoiminen salasanan nollaaminen (SSPR) ongelmia?
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002464"
- "7663"
ms.openlocfilehash: bd76ae6b2ce140fd8feb490a5fffe1baa36598e7650107f176baec30d71b8628
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945847"
---
# <a name="having-self-service-password-reset-sspr-problems"></a>Onko omatoiminen salasanan nollaaminen (SSPR) ongelmia?

Yleisiä SSPR (Self-service password reset) -ongelmia pilvipalvelujen yhdistelmäympäristössä ja paikallisissa ympäristöissä ovat:

- [SSPR-salasanan takaisinkirjaaminen ei ole käytössä](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)
- [Azure AD Premium -käyttöoikeutta ei ole määritetty](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing)
- [Azure AD:Näyttöyhteys tai](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) [verkko-ongelmat](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-connectivity)
- [SSPR-todennusmenetelmät, jotka eivät ole rekisteröityjä](https://mysignins.microsoft.com/security-info)
- [Kirjoitusta ei tueta -skenaariot,](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-writeback#unsupported-writeback-operations) kuten Microsoft 365 -hallinta tai järjestelmänvalvojat, jotka käyttävät SSPR:tä


Lisätietoja on seuraavissa artikkeleissa:

- [Omatoiminen salasanan vaihtotoiminnon vianmääritys](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr)
- [Omatoiminen salasanan palauttamisen palautustoiminnon vianmääritys Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)
