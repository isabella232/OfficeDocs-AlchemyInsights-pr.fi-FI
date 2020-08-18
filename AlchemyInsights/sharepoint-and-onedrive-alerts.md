---
title: Viiveet SharePoint-ja OneDrive-ilmoitusten vastaanottamisessa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 92e517ae6e83aa91b9838047ec77759dc893bc57
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/17/2020
ms.locfileid: "46785662"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>Viiveet SharePoint-ja OneDrive-ilmoitusten vastaanottamisessa

- Tarkista ensin roska posti-tai roska posti-kansio sähkö postista.
- Jos **Kaikki useiden tiedostojen tai kirjastojen ilmoitukset viivästyvät**, tarkista [palvelun kunnon koonti näytöstä](https://portal.office.com/adminportal/home?ref=/servicehealth) , että SharePoint-tai Exchange-palvelussa mahdollisesti esiintyvät varoitukset ja häiriöt ovat mahdollisia. Ongelma voi olla SharePoint-ilmoitusten ominaisuus tai viiveet Sähkö posti viesteissä Exchangen kautta. Huomaa myös, onko muita Sähkö posti viestejä toimitettu – jos näin ei ole, ongelma aiheutuu todennäköisesti Exchange-viiveistä.
- Jos **tietyn tiedoston tai kirjaston yksittäistä ilmoitusta ei toimiteta**, yritä poistaa se ja luoda se uudelleen. Jos haluat luoda ilmoituksen uudelleen [, Katso SharePoint-ilmoitusten hallinta, tarkastelu tai poistaminen](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) .

> [!NOTE]
> - Hälytyksiä ei voi lähettää jakelun ryhmälle. Vain suojausta ja O365 ryhmiä tuetaan.
> - Et voi mukauttaa ilmoitusten Sähkö posti malleja. Sinun on käytettävä Microsoft Flow'ta tai SharePoint Designer-työn kulkua niiden saavuttamiseksi.
