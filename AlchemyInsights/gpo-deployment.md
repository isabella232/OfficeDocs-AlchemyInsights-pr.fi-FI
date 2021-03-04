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
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427255"
---
# <a name="gpo-deployment"></a>GPO-käyttöönotto

Käyttäjä- ja tietokoneobjektien asetuksia Azure Active Directory -toimialueen palveluissa (Azure AD DS) hallitaan usein ryhmäkäytäntöobjektien (GPOs) avulla. Azure AD DS sisältää sisäänrakennettuja GPOs-objekteja AADDC-käyttäjille ja AADDC-tietokonesäilöille. Voit mukauttaa näitä sisäänrakennettuja ryhmäkäytäntöobjekteja ja määrittää ryhmäkäytännön tarpeen mukaan ympäristössäsi. Azure AD DC -järjestelmänvalvojien ryhmän jäsenillä on ryhmäkäytäntöjen hallinnan oikeudet Azure AD DS -toimialueella, ja he voivat myös luoda mukautettuja ryhmäkäytäntöjä ja organisaatioyksiköitä. Lisätietoja ryhmäkäytännön toiminnasta on ryhmäkäytännön [yleiskatsauksessa.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

Yhdistelmäympäristössä paikalliseen AD DS -ympäristöön määritettyjä ryhmäkäytäntöjä ei synkronoida Azure AD DS:n kanssa. Voit määrittää käyttäjien tai tietokoneiden määritysasetukset Azure AD DS:ssä muokkaamalla yhtä oletusarvoista ryhmäkäytäntöobjektia tai luomalla mukautetun ryhmäkäytäntöobjektin.

Tässä artikkelissa [ryhmäkäytännön hallinta](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) näyttää, miten voit asentaa ryhmäkäytäntöjen hallintatyökalut, miten voit muokata sisäänrakennettuja ryhmäkäytäntöobjekteja ja luoda mukautettuja ryhmäkäytäntöobjekteja.
