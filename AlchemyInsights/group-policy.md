---
title: Ryhmäkäytäntö
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256715"
---
# <a name="group-policy"></a>Ryhmäkäytäntö

Käyttäjä- ja tietokoneobjektien asetuksia Azure Active Directory -toimialueen palveluissa (Azure AD DS) hallitaan usein ryhmäkäytäntöobjektien (GPOs) avulla. Azure AD DS sisältää sisäänrakennettuja GPOs-objekteja AADDC-käyttäjille ja AADDC-tietokonesäilöille. Voit mukauttaa näitä sisäänrakennettuja ryhmäkäytäntöobjekteja ja määrittää ryhmäkäytännön tarpeen mukaan ympäristössäsi. Azure AD DC -järjestelmänvalvojien ryhmän jäsenillä on ryhmäkäytäntöjen hallinnan oikeudet Azure AD DS -toimialueella, ja he voivat myös luoda mukautettuja ryhmäkäytäntöjä ja organisaatioyksiköitä. Lisätietoja ryhmäkäytännön toiminnasta on ryhmäkäytännön [yleiskatsauksessa.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

Yhdistelmäympäristössä paikalliseen AD DS -ympäristöön määritettyjä ryhmäkäytäntöjä ei synkronoida Azure AD DS:n kanssa. Voit määrittää käyttäjien tai tietokoneiden määritysasetukset Azure AD DS:ssä muokkaamalla yhtä oletusarvoista ryhmäkäytäntöobjektia tai luomalla mukautetun ryhmäkäytäntöobjektin.

Tässä artikkelissa [ryhmäkäytännön hallinta](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) näyttää, miten voit asentaa ryhmäkäytäntöjen hallintatyökalut, miten voit muokata sisäänrakennettuja ryhmäkäytäntöobjekteja ja luoda mukautettuja ryhmäkäytäntöobjekteja.



