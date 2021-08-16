---
title: Ryhmien määrittäminen Azure AD -rooliin
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
- "7898"
- "9003230"
ms.openlocfilehash: 563b1a7c93c9ca64fdea51c57b70fd2132750c4ad8ee15de0c65c9668c9c3c56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036237"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Ryhmien määrittäminen Azure AD -rooliin

Jos haluat määrittää Azure AD -ryhmän, jonka myöntäjänä on Azure AD, Azure AD -rooliin, toimi seuraavasti:

1. Luo uusi ryhmä – Luo uusi ryhmä:

    a. Kirjaudu Azure AD -hallintakeskukseen järjestelmänvalvojan **tai** yleisen **järjestelmänvalvojan käyttöoikeuksilla.**
    b. Valitse **Azure Active Directory > ryhmät > Kaikki ryhmät -> Uusi ryhmä**.
    c. Luo ryhmä.

2. Määritä ryhmälle rooli joko ryhmän luomisen aikana tai sen luomisen jälkeen.

    a. Jos haluat määrittää ryhmälle roolin ryhmän luomisen yhteydessä, voit määrittää ryhmälle **azure AD** -roolien vaihtopainikkeen ja luoda ryhmän.
    b. Jos haluat määrittää ryhmälle roolin sen luomisen  jälkeen, siirry uuden luodun ryhmän Määritetyt roolit -välilehteen ja määritä ryhmälle rooli.  

**Azure AD -rooliin määritetyn ryhmän jäsenyyden hallinta**

Oletusarvoisesti vain järjestelmänvalvojat ja yleiset järjestelmänvalvojat voivat estää oikeuksien laajentamisen muokkaamalla rooliin määritetyn ryhmän jäsenyyttä. He voivat kuitenkin määrittää omistajan tälle ryhmälle ja delegoida tämän tehtävän.

Lisätietoja pilviryhmien määrittämisestä Azure AD -rooleille on kohdassa [AD-roolien määrittäminen pilviryhmälle.](https://docs.microsoft.com/azure/active-directory/roles/groups-concept) Lisätietoja pilviryhmille määritettyjen roolien vianmäärityksestä on kohdassa [Pilviryhmille määritettyjen roolien vianmääritys.](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)





