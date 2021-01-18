---
title: Toimialueen palvelun määrittäminen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885224"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>AAD-DS:n käyttöönotto ei onnistu tai käyttöönotto epäonnistuu

Voit ratkaista Azure AD -toimialueen palvelun (AAD-DS) käyttöönoton epäonnistumisen tai sen, että sitä ei ole otettu käyttöön, toimimalla seuraavasti:

1. Jos käytät jo olemassa olevaa näennäisverkkoa, tarkista NSG:stä säännöt, jotka estävät portit, joita tarvitaan portaalin AAD-DS-synkronointiin. https://aka.ms/aadds-networking
2. Tarkista, onko virheilmoitukseen vastattu tässä vianmääritysoppaassa, joka on käytettävissä  https://aka.ms/aadds-troubleshoot-enable .
3. Kokeile Azure AD -toimialueen palvelujen käyttöönottoa uudessa virtuaaliverkossa.
4. Tutustu AAD-DS:n käyttöönottoon aloitusoppaassa: [AAD-toimialuepalvelujen](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)luominen ja määrittäminen.
5. Jos sinulla on ongelmia Azure AD -toimialuepalvelujen käyttöönotossa, katso [Azure AD -toimialueen](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) palveluiden vianmääritys ja ratkaise yleisiä virheitä, jotta saat asiat toimimaan uudelleen. 

**AAD-DS:n poistaminen käytöstä ei onnistu**

AAD-DS:tä ei voi keskeyttää. Jos haluat lopettaa hallitun toimialueen käytön, se on poistettava.
Jos haluat poistaa hallitun toimialueen, katso [kohta AAD-toimialueen palvelun poistaminen.](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds)



