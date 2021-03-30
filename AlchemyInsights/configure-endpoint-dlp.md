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
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402417"
---
# <a name="configure-endpoint-dlp"></a>Määritä päätepisteen DLP

Microsoftin päätepisteen DLP sallii sinun laajentaa tietojen menetyksen estämisen suojausta ja arkaluonteisten tietojen valvontakykyä Windows 10 -laitteissa. Kun laitteet on otettu käyttöön laitteiden hallinnassa, voit luoda DLP-käytäntöjä kohteiden suojaustoimiin. Toiminnan hallinnassa voit valvoa arkaluonteisten kohteiden toimintaa. Lisätietoja on kohdassa [Laitteiden käyttöönotto laitteiden hallinnassa](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Jos haluat aloittaa päätepisteen DLP:n käytön:

- Varmista, että sinulla on tarvittavat SKU- tai tilauskäyttöoikeudet. Lisätietoja on kohdassa [SKU- tai tilauskäyttöoikeudet](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Tarkista käyttöoikeudet, jotka vaaditaan laitteiden hallintaan, laitteiden lisäyssivulle pääsyyn tai laitteiden valvonnan käyttöönottoon tai sen käytöstä poistamiseen. Lisätietoja on kohdassa [Käyttöoikeudet](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Lisää laitteita laitteiden hallintaan noudattamalla laitteiden käyttöönoton toimintosarjaa. Jos laitteiden käyttöönotto (esikatselu) puuttuu M365:n **yhteensopivuusasetuksista**, varmista, että sinulla on edellä mainitut käyttöoikeudet. Lisätietoja on kohdassa [Laitteiden käyttöönotto](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Luo DLP-käytäntöjä arkaluonteisten kohteiden suojaamiseksi. Lisätietoja on kohdassa [Päätepisteen DLP-käytäntöjen skenaarioita](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).

Lisätietoja Microsoftin päätepisteen DLP:stä on kohdassa [Microsoft 365:n päätepisteiden tietojen menetyksen estäminen (esikatselu)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Tärkeät tietojen keräysvaiheet, jos tukea tarvitaan:**

1. Lataa MDATP Client Analyzer Preview: [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")
2. Suorita työkalu järjestelmänvalvojana komentoikkunassa:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. Kun näyttöön tulee kehote antaa seurantalokien keräämisen minuuttimäärä, syötä skenaarion suorittamiseen vaadittava minuuttimäärä.
5. Suorita skenaario

Ota talteen tukiedustajalle annettava zip-tiedosto.
