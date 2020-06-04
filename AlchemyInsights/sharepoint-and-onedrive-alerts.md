---
title: SharePoint- ja OneDrive-ilmoitusten vastaanottamisen viivästyminen
ms.author: v-todmc
author: todmccoy
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
ms.openlocfilehash: 7f1033cec3abec782d1eee3b32128c4c60778913
ms.sourcegitcommit: 8e093114cd31141664e267a7c7b779398d5fdfa8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/04/2020
ms.locfileid: "44563507"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>SharePoint- ja OneDrive-ilmoitusten vastaanottamisen viivästyminen

- Tarkista ensin sähköpostisi Roskaposti- tai Roskaposti-kansio.
- Jos **kaikki useiden tiedostojen tai kirjastojen ilmoitukset viivästyvät,** tarkista [Palvelun kunnon koontinäytöstä](https://portal.office.com/adminportal/home?ref=/servicehealth) sharepointin tai Exchangen kanssa mahdollisesti ilmenevät tiedotteet/tapahtumat. Ongelma saattaa johtua SharePoint-hälytysominaisuudesta tai viiveistä sähköpostiviesteissä Exchangen kautta. Huomaa myös, toimitetaanko muita sähköpostiviestejä – jos ei, ongelma liittyy todennäköisesti Exchange-viiveisiin.
- Jos **tietyn tiedoston tai kirjaston yksittäistä ilmoitusta ei toimiteta,** yritä poistaa se ja luoda se uudelleen. Lisätietoja ilmoituksen luomisesta on kohdassa [SharePoint-ilmoitusten hallinta, tarkasteleminen tai poistaminen.](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)

> [!NOTE]
> - Ilmoituksia ei voi lähettää jakeluryhmään. Vain Suojaus- ja O365-ryhmiä tuetaan.
> - Hälytyssähköpostimalleja ei voi mukauttaa. Sinun on käytettävä Microsoft Flow'n tai SharePoint Designerin työnkulkua näiden tavoitteiden saavuttamiseksi.
