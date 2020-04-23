---
title: SharePoint- ja OneDrive-ilmoitusten vastaanottamisen viivästykset
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
ms.openlocfilehash: fb7ab6e8139c46d89b1cae1ee0ab9b9a601c8b64
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741998"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a>SharePoint- ja OneDrive-ilmoitusten vastaanottamisen viivästykset

- Tarkista ensin roskapostikansio sähköpostistasi.
- Jos **kaikki useiden tiedostojen tai kirjastojen ilmoitukset viivästyvät,** tarkista, onko SharePointissa tai Exchangessa mahdollisesti ilmenneitä tietoja tai tapahtumia Palvelun [kunto -koontinäytössä.](https://portal.office.com/adminportal/home?ref=/servicehealth) Ongelma saattaa johtua SharePoint-hälytysominaisuudesta tai viiveistä Exchangen kautta. Huomaa myös, toimitetaanko muita sähköpostiviestejä – jos ei, ongelma liittyy todennäköisesti Exchange-viiveisiis.
- Jos **tietyn tiedoston tai kirjaston yksittäistä ilmoitusta ei toimiteta,** yritä poistaa se ja luoda se uudelleen. Lisätietoja ilmoituksen luomisesta on ohjeaiheessa [SharePoint-ilmoitusten hallinta, tarkasteleminen tai poistaminen.](https://support.microsoft.com/office/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)

> [!NOTE]
> - Hälytyksiä ei voi lähettää jakeluryhmään. Vain suojaus- ja O365-ryhmiä tuetaan.
> - Hälytyssähköpostimalleja ei voi mukauttaa. Sinun on käytettävä Microsoft Flow'ta tai SharePoint Designer -työnkulkua.
