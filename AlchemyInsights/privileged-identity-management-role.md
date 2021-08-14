---
title: Privileged Identity Management rooli
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
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973226"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management(PIM) -rooli

**Käyttöoikeuksia ei myönnetä roolin aktivoinnin jälkeen**

Kun aktivoit roolin Azure AD Privileged Identity Management (PIM) -palvelussa, aktivointi ei välttämättä välittömästi välity kaikkiin portaaleihin, jotka edellyttävät järjestelmän privileged -roolia. Joskus, vaikka muutos välitisi, portaalin verkkovälimuistin tallentaminen saattaa aiheuttaa sen, että muutos ei tule voimaan välittömästi.

Jos aktivointi viivästyy, toimi seuraavasti:

1. Kirjaudu ulos Azure-portaalista ja kirjaudu sitten takaisin sisään. Kun aktivoit Azure AD -roolin tai Azure-resurssiroolin, näet aktivoinnin vaiheet. Kun kaikki vaiheet on suoritettu, näet Kirjaudu ulos -linkin. Tämän linkin avulla voit kirjautua ulos. Tämä ratkaisee useimmat aktivointiviiveen tapaukset.
2. Varmista PIM-kohdassa, että sinut on lueteltu roolin jäsenenä.
3. Jos aktivoit järjestelmänvalvojan Exchange, varmista, että kirjaudut ulos ja kirjaudut takaisin sisään. Jos ongelma jatkuu, avaa tukipalvelupyynnön ja ota tämä esille ongelmana. Jos käytät tietoturva- Exchange-järjestelmänvalvojan roolia, katso seuraavaa vaihetta.
4. Jos olet aktivoimassa roolia käyttöoikeus- ja yhteensopivuuskeskuksen käyttöön tai jos aktivoit SharePoint-järjestelmänvalvojan roolia, aktivointiviive on muutaman minuutin ja muutaman tunnin kuluttua. Tämä on tunnettu ongelma, ja työskentelemme aktiivisesti näiden tiimien kanssa ongelman ratkaisemiseksi mahdollisimman pian.

Lisätietoja on seuraavissa artikkeleissa:

- [Azure AD -roolien aktivoiminen PIM-palvelussa](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [Azure-resurssiroolien aktivoiminen PIM:ssä](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**Käyttöoikeuksia ei poisteta roolin aktivoinnin poistamisen jälkeen tai roolin aktivointi vanhenee**

Kun poistat roolin aktivoinnin Azure AD Privileged Identity Management tai kun roolin aktivointijakso päättyy, käyttöoikeus voi jatkua viiveellä.

Jos aktivoinnin poisto viivästyy, toimi seuraavasti:

1. Jos olet poistamassa Exchange-järjestelmänvalvojan roolin aktivointia tai roolin aktivointijakso vanhenee ja huomaat huomattavan viiveen ennen käyttöoikeuksien poistamista, avaa tukipalvelupyynnön ja pyydä tukihenkilöä auttamaan sinua jakamaan lippu Privileged Access Management (PAM) -työryhmälle Office tietoja tästä ongelmasta.
2. Jos aktivointijakso on päättynyt, mutta selainistunto on edelleen avoinna, sulje selain. Voit jatkaa roolin käyttöä, kunnes suljet istunnon. Tämä on tunnettu ongelma, ja microsoft tarkastelee mahdollista korjausta jokaisen istunnon aktiiviseen peruuttamista varten, kun aktivointi on päättynyt.

Jos viive on eri kuin nämä kaksi skenaariota, avaa tukipalvelupyynnön.
