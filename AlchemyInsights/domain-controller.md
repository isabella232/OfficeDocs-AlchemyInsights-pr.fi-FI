---
title: Toimialueen ohjauskone
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901022"
---
# <a name="domain-controller"></a>Toimialueen ohjauskone

**AAD-DS:n käyttöönotto ei onnistu tai käyttöönotto epäonnistuu**

Voit ratkaista Azure AD -toimialueen palvelun (AAD-DS) käyttöönoton epäonnistumisen tai sen, että sitä ei ole otettu käyttöön, toimimalla seuraavasti:

1. Jos käytät jo olemassa olevaa näennäisverkkoa, tarkista NSG:stä säännöt, jotka estävät portit, joita tarvitaan portaalin AAD-DS-synkronointiin. https://aka.ms/aadds-networking
2. Tarkista, onko virheilmoitukseen vastattu tässä vianmääritysoppaassa, joka on käytettävissä  https://aka.ms/aadds-troubleshoot-enable .
3. Kokeile Azure AD -toimialueen palvelujen käyttöönottoa uudessa virtuaaliverkossa.
4. Katso aloitusoppaasta, miten voit ottaa käyttöön AAD-DS:n, joka on saatavilla Azure AD -toimialuepalvelujen luontia [varten opetusohjelmassa.](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)
5. Jos sinulla on ongelmia Azure AD -toimialuepalvelujen käyttöönotossa, katso [Azure AD -toimialueen](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) palveluiden vianmääritys ja ratkaise yleisiä virheitä, jotta saat asiat toimimaan uudelleen. 

**AAD-DS:n poistaminen käytöstä ei onnistu**

AAD-DS:tä ei voi keskeyttää. Jos haluat lopettaa hallitun toimialueen käytön, se on poistettava.

Jos ongelmia ilmenee, voit ratkaista yleisiä virhesanomia ja ohjeita vianmääritykseen, joiden avulla saat asiat taas toimimaan, artikkelista Azure Active Directory -toimialueen palveluiden [vianmääritys.](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot)
