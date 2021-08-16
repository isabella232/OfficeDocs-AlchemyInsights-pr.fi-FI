---
title: GPO-käyttöönotto
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067837"
---
# <a name="gpo-deployment"></a>GPO-käyttöönotto

Asetukset ja tietokoneobjekteja Azure Active Directory Domain Services -palveluissa (Azure AD DS) hallitaan usein ryhmäkäytäntöobjektien (GPOs) avulla. Azure AD DS sisältää sisäänrakennettuja säilöjä AADDC-käyttäjille ja AADDC-tietokonesäilöille. Voit mukauttaa näitä sisäänrakennettuja ryhmäkäytäntöobjekteja niin, että ryhmäkäytäntö määritetään ympäristössä tarpeen mukaan. Azure AD:n dc-järjestelmänvalvojien ryhmällä on ryhmäkäytännön hallinnan oikeudet Azure AD DS -toimialueeseen, ja he voivat myös luoda mukautettuja ryhmäkäytäntöjä ja organisaation yksiköitä (OU). Lisätietoja ryhmäkäytännön toiminnasta ja toiminnasta on ryhmäkäytännön [yleiskatsauksessa.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

Yhdistelmäympäristössä paikalliseen AD DS -ympäristöön määritettyjä ryhmäkäytäntöjä ei synkronoida Azure AD DS:n kanssa. Voit määrittää käyttäjien tai tietokoneiden määritysasetukset Azure AD DS:ssä muokkaamalla yhtä oletusarvoista ryhmäkäytäntöobjektia tai luomalla mukautetun ryhmäkäytäntöobjektin.

Tässä artikkelissa [ryhmäkäytännön hallinta](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) on ohjeet ryhmäkäytäntöjen hallintatyökalujen asentamiseen, valmiin ryhmäkäytäntöobjektien muokkaamisen ja mukautettujen ryhmäkäytäntökäytäntöjen luomiseen.
