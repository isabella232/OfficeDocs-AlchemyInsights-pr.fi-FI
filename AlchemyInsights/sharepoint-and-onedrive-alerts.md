---
title: Viiveet SharePoint-ja OneDrive-ilmoitusten vastaanottamisessa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727240"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Viiveet SharePoint-ja OneDrive-ilmoitusten vastaanottamisessa

- Tarkista ensin roska posti-tai roska posti-kansio sähkö postista.
- Jos **Kaikki useiden tiedostojen tai kirjastojen ilmoitukset viivästyvät**, tarkista [palvelun kunnon koonti näytöstä](https://portal.office.com/adminportal/home?ref=/servicehealth) , että SharePoint-tai Exchange-palvelussa mahdollisesti esiintyvät varoitukset ja häiriöt ovat mahdollisia. Ongelma voi olla SharePoint-ilmoitusten ominaisuus tai viiveet Sähkö posti viesteissä Exchangen kautta. Huomaa myös, onko muita Sähkö posti viestejä toimitettu – jos näin ei ole, ongelma aiheutuu todennäköisesti Exchange-viiveistä.
- Jos **tietyn tiedoston tai kirjaston yksittäistä ilmoitusta ei toimiteta**, yritä poistaa se ja luoda se uudelleen. Jos haluat luoda ilmoituksen uudelleen [, Katso SharePoint-ilmoitusten hallinta, tarkastelu tai poistaminen](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) .

> [!NOTE]
> - Hälytyksiä ei voi lähettää jakelun ryhmälle. Vain suojausta ja O365 ryhmiä tuetaan.
> - Et voi mukauttaa ilmoitusten Sähkö posti malleja. Sinun on käytettävä Microsoft Flow'ta tai SharePoint Designer-työn kulkua niiden saavuttamiseksi.
