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
ms.openlocfilehash: f29d8476881fb3f93b369c057efed0acdd2169baf956ab43bf3c0ade527e9437
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54033527"
---
# <a name="configure-endpoint-dlp"></a>Määritä päätepisteen DLP

Microsoftin päätepisteen DLP sallii sinun laajentaa tietojen menetyksen estämisen suojausta ja arkaluonteisten tietojen valvontakykyä Windows 10 -laitteissa. Kun laitteet on otettu käyttöön laitteiden hallinnassa, voit luoda DLP-käytäntöjä kohteiden suojaustoimiin. Toiminnan hallinnassa voit valvoa arkaluonteisten kohteiden toimintaa. Lisätietoja on kohdassa [Laitteiden käyttöönotto laitteiden hallinnassa](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Jos haluat aloittaa päätepisteen DLP:n käytön:

- Varmista, että sinulla on tarvittavat SKU- tai tilauskäyttöoikeudet. Lisätietoja on kohdassa [SKU- tai tilauskäyttöoikeudet](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Tarkista käyttöoikeudet, jotka vaaditaan laitteiden hallintaan, laitteiden lisäyssivulle pääsyyn tai laitteiden valvonnan käyttöönottoon tai sen käytöstä poistamiseen. Lisätietoja on kohdassa [Käyttöoikeudet](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Lisää laitteita laitteiden hallintaan noudattamalla laitteiden käyttöönoton toimintosarjaa. Lisätietoja on kohdassa [Laitteiden käyttöönotto](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Luo DLP-käytäntöjä arkaluonteisten kohteiden suojaamiseksi. Lisätietoja on kohdassa [Päätepisteen DLP-käytäntöjen skenaarioita](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Lisätietoja Microsoftin päätepisteen DLP:stä on kohdassa [Microsoft 365:n päätepisteiden tietojen menetyksen estäminen (esikatselu)](/microsoft-365/compliance/endpoint-dlp-learn-about).

**Tärkeät tietojen keräysvaiheet, jos tukea tarvitaan:**

1. Lataa [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).
1. Suorita työkalu järjestelmänvalvojana komentoikkunassa:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Kun näyttöön **tulee Anna seurantalokien keräämiseen tarvittava minuuttimäärä:**, kirjoita skenaarion suorittamiseen tarvittava minuuttimäärä.
1. Suorita skenaario.

Kerää Zip-tiedoston tuloste tukiedustajalle annettavaksi.
