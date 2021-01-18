---
title: LDAP:n määrittäminen
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
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885159"
---
# <a name="configure-ldap"></a>LDAP:n määrittäminen

Voit määrittää LDAP:n seuraavasti:

1. Tarkista toimialueesi kunto [Azure-portaalissa.](https://aka.ms/aadds-health)
1. Varmista, että kelvollinen Azure AD -tilaus on saatavilla ja Azure AD -toimialueen palvelut on otettu käyttöön.
1. Suojatun LDAP-järjestelmän käyttöönottoon tarvittava varmenne on hankittava luotettavalta julkiselta varmenteen myöntäjältä tai itse allekirjoitettu varmenne.
1. Varmista, että varmenne noudattaa tarvittavia [ohjeita.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)

**Virheellinen varmenne**
1. Jos haluat uusia varmenteen, luo uusi varmenne ja lataa se uudelleen noudattamalla ohjeita: [LDAP:n määrittäminen.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
1. Lisätietoja suojatun LDAP-ilmoitusten tunnetun ongelman ratkaisemisesta Azure Active Directory -toimialueen palveluissa on [ohjeaiheessa LDAP-ilmoitusten ratkaiseminen.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support)
