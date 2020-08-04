---
title: Ongelmia Intune-hallintakonsolin käytössä
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555038"
---
# <a name="problems-using-the-intune-admin-console"></a>Ongelmia Intune-hallintakonsolin käytössä

**"Käyttö estetty" siirryttäessä Intune-hallintaportaaliin.**

- Jos olet Intune-mukautetun roolin jäsen, varmista, että tilillesi on määritetty Intune- tai Enterprise Mobility Suite (EMS) -käyttöoikeus.
- Jos käytät Configuration Manageria laitteiden hallintaan, varmista, ettet ole osa Configuration Managerin MDM:n Intune-käyttäjäkokoelmaa.
- Varmista, että sinulle on määritetty asianmukaiset roolipohjaiset hallintaoikeudet (RBAC) Intune roles -terässä.
- Varmista, että käytetty ryhmä ei ole jakeluluettelo. Azure-portaalin Intune tukee vain Azure Active Directory -käyttöoikeusryhmiin kuuluvia käyttäjätilejä. Tarkastele ryhmiä Azure-portaalissa > **Intune**  >  **Groupsissa**tai Azure-portaalissa > **Azure Active Directoryssa**.

**Käyttäjällä on liian monta intune-roolin käyttöoikeuksia**

Kehota käyttäjää siirtymään **Intune**  >  **Intune -rooleihin**  >  **Omat oikeudet**  >  **Vie** tarkistaaksesi myönnetyt käyttöoikeudet.

**Lisäsin rooliin vaikutusalueryhmän, mutta kyseisen roolin käyttäjät näkevät edelleen muita käyttäjiä tai laitteita.**

Vaikutusalueryhmät eivät suodata käyttäjiä tai laitteita. Vaikutusalueryhmät:

- Rajoita, kenelle käyttäjät voivat määrittää käytäntöjä tai sovelluksia.
- Salli vain tiettyjen käyttäjien suorittaa etätehtäviä laitteissa.

Lisätietoja vaikutusalueryhmistä on kohdassa [Roolipohjainen käytönvalvonta (RBAC) Ja Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Lisäsin käyttäjän Intune rooli, mutta heillä on edelleen täysi pääsy Intune admin konsoli.**

Siirry Azure-portaalin Intune > **-kohtaan** ja varmista, että käyttäjää ei ole määritetty mihinkään seuraavista azure-portaalin rooleista:

- Yleinen järjestelmänvalvoja
- Intune-palvelun järjestelmänvalvoja
- SharePoint-järjestelmänvalvoja

Lisätietoja on [ohjeaiheessa Roolipohjainen käytönvalvonta (RBAC) Ja Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Käyttöongelmat**

Lisätietoja on [ohjeaiheessa Office 365:ssä, Azuressa tai Intunessa kirjautuminen ei onnistu.](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)