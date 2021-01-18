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
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885065"
---
# <a name="assigning-groups-to-azure-ad-role"></a>Ryhmien määrittäminen Azure AD -rooliin

Voit määrittää Azure AD -ryhmän, jonka myöntäjä on Azure AD:ssä Azure AD -rooliin, toimimalla seuraavasti:

1. Uuden ryhmän luominen – Uuden ryhmän luominen:

    a. Kirjaudu Azure AD -hallintakeskukseen järjestelmänvalvojan **tai** yleisen **järjestelmänvalvojan** käyttöoikeuksilla.
    b. Valitse **Azure Active Directory > ryhmät > Kaikki ryhmät > uusi ryhmä**.
    c. Luo ryhmä.

2. Määritä ryhmälle rooli joko ryhmän luomisen tai sen luomisen jälkeen.

    a. Jos haluat määrittää ryhmälle roolin ryhmän luomisen yhteydessä, voit määrittää ryhmälle **azure AD** -roolien vaihtopainikkeen ja luoda ryhmän.
    b. Jos haluat määrittää roolin ryhmälle sen luomisen  jälkeen, siirry juuri luodun ryhmän Määritetyt roolit -välilehteen ja määritä rooli ryhmälle.  

**Azure AD -rooliin määritetyn ryhmän jäsenyyden hallinta**

Oletusarvoisesti vain järjestelmänvalvojat ja yleiset järjestelmänvalvojat voivat estää oikeuksien laajentamisen muokkaamalla rooliin määritetyn ryhmän jäsenyyttä. He voivat kuitenkin määrittää omistajalle tällaisen ryhmän ja delegoida tämän tehtävän.

Lisätietoja pilviryhmien määrittämisestä Azure AD -rooleille on kohdassa AD-roolien [määrittäminen pilviryhmälle.](https://docs.microsoft.com/azure/active-directory/roles/groups-concept) Lisätietoja pilviryhmille määritettyjen roolien vianmäärityksestä on kohdassa [Pilviryhmille määritettyjen roolien vianmääritys.](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)





