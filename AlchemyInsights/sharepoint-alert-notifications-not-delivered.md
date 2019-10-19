---
title: SharePoint-ilmoitus ilmoituksia ei toimitettu
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: d01d985f34d782fe14b3e2e6e6696c0101002db1
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/18/2019
ms.locfileid: "36744638"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>SharePoint-ilmoitus ilmoituksia ei toimitettu

Tarkista sähkö postisi roska posti kansio, sillä joskus hälytykset saattavat mennä sinne.

Selvitä, onko **kaikkia hälytyksiä toimitettu** tai onko tietyn tiedoston tai kirjaston **yksittäistä ilmoitusta** toimitettu.

- **Yksittäisiä hälytyksiä ei toimiteta**: jos tietystä tiedostosta tai kirjastosta ei toimiteta yksittäistä ilmoitusta, voit yrittää poistaa sen ja luoda sen uudelleen. Katso [SharePoint-ilmoitusten hallinta, tarkasteleminen tai poistaminen](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=&ad=US#ID0EAADAAA=Online) , jos haluat luoda hälytyksen uudelleen.
- **Kaikkia hälytyksiä ei toimiteta**: Jos kaikkia ilmoituksia useista tiedostoista tai kirjastoista ei toimiteta, käy [palvelun kunnon koonti näytössä](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) ja tarkista, onko SharePointissa tai exchangeissa mahdollisesti esiintyviä neuvoja tai tapahtumia. Ongelma saattaa olla SharePoint-hälytys ominaisuudella tai viivästyttää sähkö posteja Exchangen kautta. On myös tärkeää huomata, onko muita Sähkö posti viestin toimitetaan, ja jos ei, ongelma on todennäköisesti vaihto viivästyksiä.

Usein kysytyt kysymykset hälytyksistä:

- Ilmoituksia ei voi lähettää jakelu ryhmälle, vain suojaus-ja O365-ryhmiä tuetaan.
- Et voi mukauttaa hälytys Sähkö posti malleja; sinun on käytettävä Microsoft FLOW-tai SharePoint Designer-työn kulkua näiden tavoitteiden saavuttamiseksi.

Lisä tietoja:

- **Hälytyksen asetukset**: lisä tietoja hälytysten määrittämisestä on kohdassa [Luo ilmoitus, jos haluat saada ilmoituksen, kun tiedosto tai kansio muuttuu SharePointissa](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).
- **Hälytysten vian määritys**: lisä tietoja hälytysten vian määrityksestä on kohdassa [käyttäjät eivät saa SharePoint Online Alert-ilmoituksia](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).
- **Advanced O365 yhteensopivuuden hälytys käytännöt**: lisä tietoja näiden ilmoitusten määrittämisestä on artikkelissa [yhteensopivuuden hälytys käytännöt](https://docs.microsoft.com/office365/securitycompliance/alert-policies).
- **SharePointin ja OneDriven valvonta lokit**: lisä tietoja näiden tapahtumien noutamista on kohdassa [Etsi valvonta lokista](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
- **Kehittyneiden uhkien torjunta-ilmoitusten lähettämät hälytykset**: Katso [ATP SharePointille ja OneDriveen](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).
- **Tietojen menetyksen estämisen käytännöt lähettämät hälytykset**: Katso [Sähkö posti-ilmoitukset DLP-käytännöistä](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).

## <a name="related-topics"></a>Aiheeseen liittyviä ohjeita

Haluatko kokeilla Microsoft Flow'ta SharePoint Onlinessa?

- [Luo työn kulku](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint ja Flow](https://flow.microsoft.com//blog/sharepoint-and-flow/)
