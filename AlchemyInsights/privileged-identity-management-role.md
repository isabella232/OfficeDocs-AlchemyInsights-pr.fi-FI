---
title: Etuoikeutettu tunniste tietojen hallinta rooli
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088675"
---
# <a name="privileged-identity-managementpim-role"></a>Etuoikeutettu tunniste tietojen hallinta (PIM)-rooli

**Käyttö oikeuksia ei myönnetä roolin Akti voinnin jälkeen**

Kun Akti voit roolin Azure AD etuoikeutettu käyttäjä tietojen hallinta (PIM)-ohjelmassa, Akti vointi ei välttämättä toimi välittömästi kaikissa portaaleista, jotka edellyttävät etuoikeutettua roolia. Joskus, vaikka muutos olisi levitetty, verkko-väli muistiin tallentaminen portaalissa voi aiheuttaa sen, että muutos ei tule heti voimaan.

Jos Akti vointi viivästyy, toimi seuraavasti:

1. Kirjaudu ulos Azure-portaalista ja kirjaudu sitten takaisin sisään. Kun Akti voit Azure AD-roolin tai Azure-resurssi roolin, Akti voinnin vaiheet tulevat näkyviin. Kun kaikki vaiheet on suoritettu, näkyviin tulee Kirjaudu ulos-linkki. Tämän linkin avulla voit kirja utua ulos. Tämä ratkaisee useimmissa tapa uksissa aktivointi viiveen.
2. Varmista, että sinut on merkitty roolin jäseneksi PIM-ohjelmassa.
3. Jos Akti voit Exchange-järjestelmänvalvojaroolin, varmista, että kirja udut ulos ja kirja udut takaisin sisään. Jos ongelma jatkuu, avaa tuki pyyntö ja nosta se ongelmaksi. Jos käytät Exchange-järjestelmänvalvojien roolia tieto turva-ja yhteensopivuus keskuksen käyttämiseen, Katso seuraava vaihe.
4. Jos aktivoitan roolin tieto turva-ja yhteensopivuus keskuksen käyttöön tai Akti voit SharePoint-järjestelmänvalvojaroolin, Akti vointi viivästyy muutamasta minuutista muutamaan tuntiin. Tämä on tunnettu ongelma, ja työskentelemme aktiivisesti näiden tiimien kanssa ongelman ratkaisemiseksi mahdollisimman pian.

Lisätietoja on seuraavissa artikkeleissa:

- [Azure AD-roolien Akti voiminen PIM-ohjelmassa](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Azure-resurssi roolien Akti voiminen PIM-ohjelmassa](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Käyttö oikeuksia ei poisteta sen jälkeen, kun rooli on poistettu käytöstä tai roolin Akti vointi on vanhentunut**

Kun poistat roolin käytöstä Azure AD:ssä, joka on etuoikeutettu käyttäjä tietojen hallinta tai kun roolin aktivointi aika päättyy, sinulla voi olla viive, jossa sinulla on edelleen käyttö oikeus.

Jos Akti voinnin poistaminen viivästyy, toimi seuraavasti:

1. Jos poistat Exchange-järjestelmänvalvojaroolin Akti voinnin tai roolin aktivointi aika päättyy ja huomaat, että käyttö oikeudet ovat huomattavasti myöhässä, avaa tuki pyyntö ja pyydä tuki henkilön apua, jotta voit arkistoida lipun, jossa on Office-käyttö oikeuksien hallinnan (PAM) tiimi.
2. Jos aktivointi aika on vanhentunut, mutta selain istunto on edelleen avoinna, sulje selain. Voit jatkaa roolin käyttöä, kunnes suljet istunnon. Tämä on tunnettu ongelma, ja tarkastelemme mahdollisia korjauksia, joilla jokainen istunto peruutetaan aktiivisesti, kun Akti vointi on vanhentunut.

Jos viivästys ei ole sama kuin näissä kahdessa skenaariossa, avaa tuki pyyntö.
