---
title: LDAP-asetusten määrittäminen
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: 3f1f9728cdcfbe5676e5afc45b2afe82836fed9c8907df3559ac7daec21194ed
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090409"
---
# <a name="configure-ldap"></a>LDAP-asetusten määrittäminen

Voit määrittää LDAP:n seuraavasti:

1. Tarkista toimialueesi kunto [Azure-portaalissa.](https://aka.ms/aadds-health)
1. Varmista, että kelvollinen Azure AD -tilaus on käytettävissä ja että Azure AD -toimialueen palvelut on otettu käyttöön.
1. Suojatun LDAP-protokollan käyttöönottoon tarvittava varmenne on hankittava luotettavalta julkiselta varmenteiden myöntäjältä tai oltava itse allekirjoitettu varmenne.
1. Varmista, että varmenne noudattaa tarvittavia [ohjeita.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**Virheellinen varmenne**
1. Jos haluat uusia varmenteen, luo uusi varmenne ja lataa se uudelleen noudattamalla ohjeita: [LDAP-asetusten määrittäminen.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
1. Jos haluat ratkaista azure Active Directory -toimialueen palvelujen suojattuihin LDAP-ilmoituksiin liittyvät tunnetut ongelmat, katso [LDAP-ilmoitusten ratkaiseminen.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
