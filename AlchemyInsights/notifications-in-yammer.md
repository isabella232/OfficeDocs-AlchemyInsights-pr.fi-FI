---
title: Yammerin ilmoitukset
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002878"
- "5480"
ms.openlocfilehash: a07d5f502beb61ab130e801b0e42579718f4d175a937fee4e21ab9f7339dbffd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097195"
---
# <a name="notifications-in-yammer"></a>Yammerin ilmoitukset

Jotta saat tietoja uudesta toiminnasta seuraamissasi keskusteluissa, [Yammer lähettää ilmoituksia](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) joko sähköpostitse tai push-ilmoituksilla, jos käytät Yammeria mobiililaitteessa. Yammer lähettää oletusarvoisesti ilmoituksia monentyyppisestä toiminnasta verkostossa. Käyttäjät voivat päivittää sähköpostiasetuksiaan Yammerin verkkosivustolla. Push-ilmoituksia hallitaan mobiilisovelluksessa. 

Yammer on lisännyt tuen [Outlookin vuorovaikutteisille sähköpostiviesteille](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420). Jotkin sähköpostit (viestin kopiot) muuttuvat vuorovaikutteisiksi Outlookin verkkoversiossa. Tuleva päivitys tuo ominaisuuden muihin Outlook-versioihin.

**Yammer-ilmoitustyypit**

- Sähköpostit (ryhmän päivitykset, esimerkiksi kun joku kutsuu sinut ryhmään tai saat viestin Saapuneet-kansioosi)
- Push-ilmoitukset (lähetetään mobiililaitteeseen esimerkiksi kun sinut mainitaan tai saat viestin Saapuneet-kansioosi)
- Työpöydän ponnahdusikkunat (kun olet asentanut Yammer-työpöytäsovelluksen, se näyttää ilmoitusruutuja).
- Kelloilmoitukset (Yammerin verkkosivuilla tulevia ilmoituksia eri tapahtumista. Näihin ilmoituksiin ei välttämättä liity sähköposti- tai push-ilmoitusta.)

[Lisätietoja ilmoituksista](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996).

**Ilmoitusten hallinta**

Käyttäjien on hallittava itse omia ilmoituksiaan. Lisätietoja on artikkelissa [Yammerin sähköposti- ja mobiili-ilmoitusten ottaminen käyttöön ja poistaminen käytöstä](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996). 

Järjestelmänvalvojat eivät voi poistaa kaikkia ilmoituksia käytöstä tai hallita ilmoituksia käyttäjien puolesta. Järjestelmänvalvojat voivat [hallita sähköpostiviesteissä olevaa logoa ja sitä, täytyykö käyttäjien vahvistaa viestit](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer), jotka lähetetään sähköpostitse.

**Sähköposti-ilmoituksia lähetetty useille organisaation käyttäjille**

Joskus Yammer lähettää yksittäisen sähköposti-ilmoituksen, jonka odotettua useampi organisaation käyttäjä vastaanottaa. Näin tapahtuu, kun Yammeriin lisätään jakeluluettelo tai muu kuin yksittäinen sähköpostiosoite. Yammer ei kaikissa tapauksissa tiedä, kuuluuko sähköpostiosoite yksittäiselle käyttäjälle vai onko kyseessä sähköpostiosoite, joka toimittaa yksittäisen viestin useille vastaanottajille. Kun ongelma ilmenee, sinun tulee [poistaa kyseisen käyttäjän ja sähköpostiosoitteen aktivointi](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) Yammerissa. 

Voit vähentää ongelman toistumisen todennäköisyyttä toimimalla seuraavasti.

1. [Pakota Office 365 -käyttäjätietojen käyttöönotto](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity)Yammerissa.
2. Estä ulkoisia lähettäjiä lähettämästä sähköpostia organisaation tai rajoita lähettäjien määrää sallittujen lähettäjien luetteloon.

Jos ongelma esiintyy:

1. Tunnista sähköpostiosoitteen vastaanottaja, jonka tulisi vastata käyttäjää Yammerissa. Esimerkiksi myyntihenkilöstö@fabrikam.com on jakeluluettelo kaikelle myyntihenkilöstölle. Tämän jakeluluettelon voi tunnistaa käyttäjien vastaanottamasta Yammer-viestistä.
2. Käytä [verkoston järjestelmänvalvojan aktivoinnin poisto-ominaisuutta](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) poistaaksesi käytöstä käyttäjän, joka käyttää osoitetta myyntihenkilöstö@fabrikam.com. Käytöstä poistamisen voi kumota, joten se on poistamista turvallisempaa. Käyttäjä poistetaan automaattisesti 90 päivän kuluttua.
3. Vaihtoehtoisesti voit tutustua artikkeliin [Käyttäjän vienti](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers) tunnistaaksesi muita muiden kuin käyttäjien sähköpostiosoitteita, jotka tulisi poistaa käytöstä.
