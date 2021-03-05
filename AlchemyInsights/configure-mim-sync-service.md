---
title: MIM-synkronointipalvelun määrittäminen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481352"
---
# <a name="configure-mim-sync-service"></a>MIM-synkronointipalvelun määrittäminen

Microsoft Identity Manager (MIM) -synkronointipalvelu on MIM:n osa. Se on keskitetty paikallinen palvelu, joka tallentaa ja integroi tietoja organisaatioille, joissa on useita paikallisia hakemistoja ja tietokantoja. Voit ehkä ratkaista MIM Sync -ongelman, jos ongelma on ratkaistu MIM:n viimeisimmässä päivityksessä tai jossakin muissa alla olevassa osiossa mainituista ongelmista.

**Suositellut vaiheet**

1. Varmista, että käytät MIM Syncin viimeaikaista päivitystä, ja tarkista [MIM Syncin julkaisutiedot](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) ja selvitä, onko ongelma korjattu päivityksessä.
2. Jos ongelma liittyy Generic LDAP-, Generic SQL-, Lotus Domino- tai Web Services -yhdistimeen, varmista, että käytät yleisten yhdistimien [viimeaikaista päivitystä.](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)
3. Jos MIM-synkronointi suoritetaan, jossa on virhe, [](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) selvitä mahdolliset syyt suorita-virhekoodien taulukosta.
4. Jos run stops with **extension-dll-exception,** then click on those words to open the **Connector Space Object properties** window, and click on Stack **Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception.](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx)
5. Jos PCNS (Password Change Notification Service) -komponentti ilmoittaa virheestä **6025** tapahtumalokissa salasanasynkronoinnin aikana, tarkista [PCNS-raportointivirheen 6025 vianmääritys oppaasta.](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)
6. Jos täydellinen synkronointi FIM-palvelun hallintaagentin  kanssa on hidasta, tarkista TempDB:n automaattinen kasvu -asetus, joka on kuvattu kohdassa Täyden synkronoinnin vianmääritys tai koko synkronoinnin [riippuvan vianmäärityksen ohje.](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)
7. Jos kohtaat virheen, jossa pysäytetty palvelin ja epäonnistunut luominen www-palvelujen kautta FIM-palvelun hallintaagentin avulla, katso [tukitiedot: via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) -palveluiden kautta epäonnistunut luominen, jossa on yleiskuvaus syistä.

