---
title: SharePoint-ja OneDrive-hälytyksiä ei saada
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/25/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 80423791ad558fc414d50608c73f823036432e14
ms.sourcegitcommit: 5e6a805fb0b41d714ca1cf90e23b8e2daa90f90e
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/26/2019
ms.locfileid: "37205519"
---
# <a name="not-receiving-sharepoint-and-onedrive-alerts"></a>SharePoint-ja OneDrive-hälytyksiä ei saada

Tarkista ensin sähkö postisi roska posti-tai roska posti kansio.

Selvitä sitten, onko **kaikkia hälytyksiä toimitettu** vai ei, jos tietystä tiedostosta tai kirjastosta ei toimiteta **yksittäistä ilmoitusta** .

- Jos **kaikkia ilmoituksia useista tiedostoista tai kirjastoista ei toimiteta**, käy [palvelun kunnon koonti näytössä](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fadmin.microsoft.com%2FAdminPortal%2FHome%23%2Fservicehealth&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=35FUOTleK0Sc0z%2B7N7Vm0tOgXplyeOe3LcIzqRziGXc%3D&reserved=0) ja tarkista, onko SharePoint-tai Exchange-palvelussa mahdollisesti ilmenneitä neuvoja tai tapahtumia. Ongelma saattaa olla SharePoint-hälytys toiminto tai sähkö postien viivästyminen Exchangen kautta. Huomaa myös, onko muita Sähkö posti viestin toimitetaan – jos ei, ongelma on todennäköisesti viivästyksiä.
- Jos **tietyn tiedoston tai kirjaston yksittäistä ilmoitusta ei toimiteta**, yritä poistaa se ja luoda se uudelleen. Katso [SharePoint-ilmoitusten hallinta, tarkasteleminen tai poistaminen](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2Fmanage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2%3Fui%3Den-US%26rs%3D%26ad%3DUS%23ID0EAADAAA%3DOnline&data=02%7C01%7Cv-todmc%40microsoft.com%7C2cd2037aa7304711d2bc08d741fae254%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C637050418099632638&sdata=AkE%2BjiG6%2BA59llp2DGcg4uHHUjaUDUnAlK5ax%2Fepn3E%3D&reserved=0) , jos haluat luoda hälytyksen uudelleen.

> [!NOTE]
> - Ilmoituksia ei voi lähettää jakelu ryhmään. Vain suojaus-ja O365-ryhmiä tuetaan.
> - Et voi mukauttaa hälytys Sähkö posti malleja. Sinun on käytettävä Microsoft Flow-tai SharePoint Designer-työn kulkua näiden tavoitteiden saavuttamiseksi.
