---
title: Adminstrators lisääminen ja hallinta – Suositellut vaiheet
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677253"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a>Adminstrators lisääminen ja hallinta – Suositellut vaiheet

**Tila uksen valvojan tai Yhteishallinnoijan muokkaaminen**

- Tilin järjestelmänvalvoja voi muokata molempia rooleja, mutta tila uksen järjestelmänvalvoja voi muuttaa vain yhteisjärjestelmänvalvojia Azure- [portaalissa](https://ms.portal.azure.com/#home).
- [Azure-tila uksen järjestelmänvalvojien lisääminen tai muuttaminen](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Tila uksen valvojan tai sisäisten (OLEVINAAN) tilausten Co-Administrator päivittäminen**

Palvelun hallinnoija tai Yhteishallinnoija voi itse palvella tätä toimintoa seuraavien vaiheiden avulla:

1. Kirjaudu sisään Azure- [portaaliin](https://ms.portal.azure.com/#home) ja valitse vasemman reunan **kustannusten hallinta + laskutus** .
2. Napsauta tilaustasi koskevaa rivi kohdetta. Tämä avaa tila uksen yleiskatsauksen.
3. Valitse **tila uksen** Blade-kohdassa **Ominaisuudet**. 
4. Napsauta **palvelun järjestelmänvalvoja** -painiketta.
5. Kirjoita sen käyttäjän Sähkö posti viesti, jonka haluat määrittää palvelun järjestelmänvalvojaksi, ja valitse **OK**.

**Yhteishallinnoijan lisääminen/muuttaminen tai poistaminen**

1. Kirjaudu [Azure-portaaliin](https://ms.portal.azure.com/#home) palvelun järjestelmänvalvojana.
2. Avaa [tila ukset](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) ja valitse tilaus. (Co-adminstrators voidaan määrittää vain tila uksen laajuus-kohdassa.)
3. Siirtyminen **käyttö oikeuksien hallintaan (IAM)**  >  **perinteiset järjestelmänvalvojat**  >  **Lisää**  >  **yhteisjärjestelmänvalvoja** -ruudun avaaminen Lisää  yhteisjärjestelmänvalvojan valinta ruutu (jos lisää yhteisjärjestelmänvalvoja-vaihto ehto ei ole käytössä, se tarkoittaa, että sinulla ei ole käyttö oikeuksia).
4. Valitse käyttäjä, jonka haluat lisätä, ja valitse **Lisää**.

**Opi lisää:**
- [Yhteishallinnoijan lisääminen](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Yhteishallinnoijan poistaminen](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Palvelun valvojan vaihtaminen](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Tilin valvojan tarkasteleminen](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Käytön hallinta RBAC-ja Azure-portaalin avulla](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Käyttäjien lisääminen tai poistaminen Azure Active Directoryssa (AD)**

Voit lisätä uusia käyttäjiä tai poistaa olemassa olevia käyttäjiä Azure Active Directory (Azure AD)-organisaatiostasi:

1. Jos haluat lisätä uuden käyttäjän, Kirjaudu [Azure-portaaliin](https://ms.portal.azure.com/#home) organisaation käyttäjä järjestelmänvalvojana.
2. Valitse **Azure Active Directory**, valitse **käyttäjät** ja valitse sitten **Uusi käyttäjä**.
3. Täytä tarvittavat tiedot **käyttäjä** -sivulla. Valitse **Luo**. Käyttäjä luodaan ja lisätään Azure AD-vuokraajaan.

Lisä **tietoja**:

- [Uuden käyttäjän lisääminen](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Käyttäjän poistaminen](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Käyttäjän profiili tietojen lisääminen tai päivittäminen Azure Active Directorya käyttäen](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Suositellut asia kirjat**

- [Mikä on roolipohjainen käytön hallinta (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Ymmärtämään eri rooleja Azuressa](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Järjestelmänvalvojaroolin käyttö oikeudet Azure Active Directoryssa](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Opetus ohjelma: käyttö oikeuksien myöntäminen käyttäjälle RBAC-ja Azure-portaalin avulla](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [RBAC-vian määritys Azuressa](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Resurssien organisointi Azure Management Groupsin avulla](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Azure-laskun kopion pyytäminen sähköpostitse](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [Luotto-tai maksu kortin lisääminen, päivittäminen tai poistaminen Azuresta](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Tila uksen hallinta (Aktivoi uudelleen/Peruuta/Vaihda)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



