---
title: Järjestelmänvalvojien lisääminen ja hallinta – suositellut vaiheet
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
ms.openlocfilehash: 48a06fde215e007b6b81b32ab751ca8e4bba522d
ms.sourcegitcommit: 46e24d65cffd37b6988447c6738b3315303bbe13
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58339029"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a>Järjestelmänvalvojien lisääminen ja hallinta – suositellut vaiheet

Ongelman kuvauksen perusteella olemme löytäneet sinulle ratkaisun. Useimmat asiakkaat pystyivät ratkaisemaan ongelmansa itse käyttöohjeiden jälkeen.

**Tilauksen järjestelmänvalvojan tai rinnakkaisvalvojan muokkaaminen**

- Tilin järjestelmänvalvoja voi muokata molempia rooleja, kun taas Tilauksen järjestelmänvalvoja voi muuttaa vain rinnakkais järjestelmänvalvojien asetuksia [Azure-portaalissa.](https://ms.portal.azure.com/#home)
- [Azure-tilauksen järjestelmänvalvojien lisääminen tai muuttaminen](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

**Päivitä tilauksen järjestelmänvalvoja tai Co-Administrator (AIRS) -tilauksia varten**

Palvelun järjestelmänvalvoja tai yhteisvalvoja voi käyttää tätä toimintoa omatoimist assa seuraavasti:

1. Kirjaudu Sisään [Azure-portaaliin ja](https://ms.portal.azure.com/#home) valitse **vasemmasta reunasta Kustannusten** hallinta + Laskutus.
2. Napsauta tilausrivin kohdetta. Tämä avaa tilauksen yleiskatsauksen.
3. Valitse **Tilaus-kohdassa** **Ominaisuudet**. 
4. Napsauta Palvelun **järjestelmänvalvoja -painiketta.**
5. Kirjoita sen käyttäjän sähköpostiosoite, jonka haluat määrittää palvelun järjestelmänvalvojaksi, ja valitse **OK.**

**Rinnakkaisvalvojan lisääminen, muuttaminen tai poistaminen**

1. Kirjaudu [Azure-portaaliin](https://ms.portal.azure.com/#home) palvelun järjestelmänvalvojana.
2. Avaa [Tilaukset](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) ja valitse tilaus. (Rinnakkaisvalvojat voidaan määrittää vain tilauksen laajuuden mukaan.)
3. Siirry kohtaan **Access control (IAM)**  >  **Classic**  >    >  administrators **Add Add co-administrator** (Lisää yhteisjärjestelmänvalvoja) ja avaa Lisää toinen järjestelmänvalvoja **-ruutu** (Jos Lisää toinen järjestelmänvalvoja -vaihtoehto ei ole käytössä, se tarkoittaa, että sinulla ei ole käyttöoikeuksia).
4. Valitse käyttäjä, jonka haluat lisätä, ja valitse **Lisää**.

**Opi lisää:**
- [Toisen järjestelmänvalvojan lisääminen](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Rinnakkaisen järjestelmänvalvojan poistaminen](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Palvelun järjestelmänvalvojan muuttaminen](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Tilin järjestelmänvalvojan tarkasteleminen](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [Käytön hallinta RBAC:n ja Azure-portaalin avulla](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

**Käyttäjien lisääminen tai poistaminen Azure Active Directory (AD)**

Voit lisätä uusia käyttäjiä tai poistaa aiemmin luotuja käyttäjiä Azure Active Directory (Azure AD) -organisaatiostasi:

1. Jos haluat lisätä uuden käyttäjän, kirjaudu [Azure-portaaliin](https://ms.portal.azure.com/#home) organisaation käyttäjänä.
2. Valitse **Azure Active Directory**, valitse **Käyttäjät** ja valitse sitten **Uusi käyttäjä**.
3. Täytä **Käyttäjä-sivulla** tarvittavat tiedot. Valitse **Luo**. Käyttäjä luodaan ja lisätään Azure AD -vuokraajaan.

**Lisätietoja:**

- [Uuden käyttäjän lisääminen](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Käyttäjän poistaminen](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [Käyttäjän profiilitietojen lisääminen tai päivittäminen Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

**Suositellut asiakirjat**

- [Mikä on roolipohjainen access control (RBAC)?](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [Eri roolien ymmärtäminen Azuressa](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [Järjestelmänvalvojan roolin käyttöoikeudet Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [Opetusohjelma: Käyttöoikeuden myöntäminen käyttäjälle, joka käyttää RBAC-menetelmää ja Azure-portaalia](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [RBAC:n vianmääritys Azuressa](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [Resurssien järjestäminen Azure-hallintaryhmien avulla](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [Azure-laskun kopion pyytäminen sähköpostitse](https://azure.microsoft.com/blog/azure-email-invoices/)
- [Luotto- tai debit-kortin lisääminen, päivittäminen tai poistaminen Azuresta](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [Tilauksen hallinta (uudelleenaktivoiminen/peruuttaminen/vaihtaminen)](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



