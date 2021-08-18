---
title: Määritä päätepisteen DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 97a8d4e7db9aac65e6a505c0bef8b41d2ea23353
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323915"
---
# <a name="configure-endpoint-dlp"></a>Määritä päätepisteen DLP

Microsoftin päätepisteen DLP sallii sinun laajentaa tietojen menetyksen estämisen suojausta ja arkaluonteisten tietojen valvontakykyä Windows 10 -laitteissa. Kun laitteet on otettu käyttöön laitteiden hallinnassa, voit luoda DLP-käytäntöjä kohteiden suojaustoimiin. Toiminnan hallinnassa voit valvoa arkaluonteisten kohteiden toimintaa. Lisätietoja on kohdassa [Laitteiden käyttöönotto laitteiden hallinnassa](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Jos haluat aloittaa päätepisteen DLP:n käytön:

- Varmista, että sinulla on tarvittavat SKU- tai tilauskäyttöoikeudet. Lisätietoja on kohdassa [SKU- tai tilauskäyttöoikeudet](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Tarkista käyttöoikeudet, jotka vaaditaan laitteiden hallintaan, laitteiden lisäyssivulle pääsyyn tai laitteiden valvonnan käyttöönottoon tai sen käytöstä poistamiseen. Lisätietoja on kohdassa [Käyttöoikeudet](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Lisää laitteita laitteiden hallintaan noudattamalla laitteiden käyttöönoton toimintosarjaa. Lisätietoja on kohdassa [Laitteiden käyttöönotto](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Luo DLP-käytäntöjä arkaluonteisten kohteiden suojaamiseksi. Lisätietoja on kohdassa [Päätepisteen DLP-käytäntöjen skenaarioita](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Lisätietoja Microsoftin päätepisteen DLP:stä on kohdassa [Microsoft 365:n päätepisteiden tietojen menetyksen estäminen (esikatselu)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Tärkeät tietojen keräysvaiheet, jos tukea tarvitaan:**

1. Lataa [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).
1. Suorita työkalu järjestelmänvalvojana komentoikkunassa:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Kun näyttöön **tulee Anna seurantalokien keräämiseen tarvittava minuuttimäärä:**, kirjoita skenaarion suorittamiseen tarvittava minuuttimäärä.
1. Suorita skenaario.

Kerää Zip-tiedoston tuloste tukiedustajalle annettavaksi.
