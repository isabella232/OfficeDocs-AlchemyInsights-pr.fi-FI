---
title: Tuominen ja vieminen Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035437"
---
# <a name="import-and-export-from-yammer"></a>Tuominen ja vieminen Yammer

**Tuo**

Käyttäjän tuontiasetukset vaihtelevat sen mukaan, onko Yammer [Microsoft 365:n](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)alkuperäinen tila vai ei.

- **Muu kuin** alkuperäinen tila: Käyttäjät voidaan tuoda ryhmiin käyttämällä Lisää osoitteistosta [-painiketta](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (100 [](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) käyttäjää) ryhmäasetuksissa tai verkostoon käyttämällä verkon järjestelmänvalvojan joukkopäivitystoimintoa.
- **Alkuperäinen tila:** Ryhmän jäsenyys- ja verkoston jäsenyystoiminnot on suoritettava [Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users)-hallintaportaalissa, [Azure AD -portaalissa](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)tai käyttämällä toista Azure AD -vaihtoehtoa. Alkuperäistilassa olevat verkostot eivät enää voi käyttää joukkopäivitystä ja muita vanhoja ominaisuuksia.

> [!IMPORTANT]
> Yammer ole koskaan tuettu sisällön tuomista verkoston järjestelmänvalvojalta, vaikka tietojen vientitoimintoa olisi käytetty toisessa verkossa. Kumppaniratkaisut tai REST-ohjelmointirajapinnat voivat Yammer uudelleen.

**Vie**

[Verkoston järjestelmänvalvojan verkostotietojen vieminen](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) sallii sisällön viennin Yammer viesteistä ja tiedostoista. Liitteet voivat olla erittäin suuria, ja viennin valmistuminen vie huomattavasti aikaa. Suosittelemme, että aktiiviset verkostot viedään [Tietojen vienti -ohjelmointirajapinnan](https://developer.yammer.com/docs/data-export-api) avulla päivittäin tai viikoittain. Microsoft-tuki ei tarjoa mukautettuja komentosarjoja tähän tarkoitukseen.

Yksittäisen käyttäjän [sisällön viemiseen](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) käytetään erillistä GDPR-vientiin.