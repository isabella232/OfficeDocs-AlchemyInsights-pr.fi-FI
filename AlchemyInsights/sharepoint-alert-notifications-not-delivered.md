---
title: SharePoint-ilmoitusilmoituksia ei toimitettu
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: a422805d11a128909e1be7bf5d08b24efc132e23
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742044"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>SharePoint-ilmoitusilmoituksia ei toimitettu

Tarkista roskapostin ROSKAPOSTI-kansio, sillä joskus hälytykset saattavat mennä sinne.

Määritä, **että kaikkia hälytyksiä ei toimiteta** tai jos tietyn tiedoston tai kirjaston **yksittäistä ilmoitusta** ei toimiteta.

- **Yksittäisiä hälytyksiä ei toimiteta:** Jos tietyn tiedoston tai kirjaston yksittäistä ilmoitusta ei toimiteta, voit yrittää poistaa sen ja luoda sen uudelleen. Lisätietoja ilmoituksen luomisesta on ohjeaiheessa [SharePoint-ilmoitusten hallinta, tarkasteleminen tai poistaminen.](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)
- **Kaikkia hälytyksiä ei toimiteta:** Jos kaikkia useiden tiedostojen tai kirjastojen ilmoituksia ei toimiteta, tarkista SharePointin tai Exchangen yhteydessä mahdollisesti ilmenevistä tiedotteista/tapahtumista [palvelun kunnon hallintapaneelista.](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) Ongelma voi johtua SharePoint-hälytysominaisuudesta tai viiveistä Exchangen kautta. On myös tärkeää huomata, toimitetaanko muuta sähköpostia, ja jos ei, ongelma liittyy todennäköisesti Exchangen viivästyksiin.

Usein kysyttyjä kysymyksiä hälytyksistä:

- Hälytyksiä ei voi lähettää jakeluryhmälle, vain suojaus- ja O365-ryhmiä tuetaan.
- Hälytyssähköpostimalleja ei voi mukauttaa. sinun on käytettävä Microsoft FLOW- tai SharePoint Designer -työnkulkua niiden saavuttamiseksi.

Lisätietoja:

- **Hälytysten asetukset**: Lisätietoja ilmoitusten määrittämisestä on [ohjeaiheessa Ilmoituksen luominen, kun tiedosto tai kansio muuttuu SharePointissa](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).
- **Ilmoitusten vianmääritys**: Lisätietoja vianmääritysilmoituksista [on ohjeaiheessa Käyttäjät eivät saa SharePoint Online -ilmoitusilmoituksia](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).
- **O365:n vaatimustenmukaisuushälytyskäytännöt**ovat kohdassa Compliance Alert [Policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies).
- **SharePointin ja OneDriven valvontalokit**: Lisätietoja näiden tapahtumien noutamisesta [on ohjeaiheessa Valvontalokin etsiminen](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
- **Advanced Threat Protectionin lähettämät hälytykset**: Katso [ATP SharePointia ja OneDrivea varten](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).
- **Tietojen menetyksen estämisen poliisien lähettämät ilmoitukset**: Katso [DLP-käytäntöjen sähköposti-ilmoitukset](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).

## <a name="related-topics"></a>Aiheeseen liittyviä aiheita

Haluatko kokeilla Microsoft Flow'ta SharePoint Onlinessa?

- [Luo työnkulku](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint ja Flow](https://flow.microsoft.com//blog/sharepoint-and-flow/)
