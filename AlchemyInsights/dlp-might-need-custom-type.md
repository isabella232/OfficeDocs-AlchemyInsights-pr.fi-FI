---
title: DLP voi tarvita mukautettua tyyppiä
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446688"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP voi tarvita mukautettua tyyppiä

**Tärkeää**: Näinä ennennäkemättöminä aikoina pyrimme varmistamaan, että SharePoint Online -ja OneDrive-palvelujen käytettävyys on hyvä. Lisätietoja on artikkelissa [SharePoint Onlinen tilapäiset ominaisuusmuutokset](https://aka.ms/ODSPAdjustments).

**DLP saattaa edellyttää mukautettua tietotyyppiä**

Tietojen menetyksen estämisen (DLP) käytännön avulla voit tunnistaa ja suojata luottamuksellisia tietoja organisaatiossasi. Joissakin tilanteissa sinun on ehkä luotava oma mukautettu luottamuksellisten tietojen tyyppi organisaatiosi tietojen suojaamiseksi. Lisätietoja on ohjeaiheessa Tietoja [luottamuksellisten tietojen tyypeistä ja](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) [Luottamuksellisten tietojen tyypin määritykset.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

Lisätietoja mukautettujen luottamuksellisten tietojen tyyppien ja käytäntöjä luodista on kohdassa: 

**Valmiin luottamuksellisen tietotyypin mukauttaminen**

Jos sisäinen luottamuksellisten tietojen tyyppi vastaa tarpeitasi muutamalla säädöllä, katso kohtaa Valmiin luottamuksellisen [tietotyypin mukauttaminen.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Voit esimerkiksi lisätä tai poistaa avainsanoja tai lisätä tai poistaa tukiaineistoa, kuten päivämäärän tai osoitteen.

**Mukautetun luottamuksellisen tietotyypin luominen**

Jos sinun on kuitenkin tunnistettava ja suojattava erityyppisiä luottamuksellisia tietoja, voit luoda mukautetun luottamuksellisen tietotyypin Microsoft 365 -yhteensopivuuskeskus. Lisätietoja on kohdassa [Mukautettujen luottamuksellisten tietotyyppien käytön aloittaminen.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)

**Mukautetun luottamuksellisen tietotyypin luominen tietoturva- & PowerShellissä**

Jos käyttöliittymässä ei ole kaikkia tarvitsemiasi asetuksia, voit luoda mukautetun luottamuksellisen tietotyypin Security & Compliance Center PowerShellissä. Kun aloitat XML-tiedostosta, voit käyttää kaikkia käytettävissä olevia vaihtoehtoja. Lisätietoja on kohdassa [Mukautetun luottamuksellisen tietotyypin luominen PowerShellin avulla.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)

Jos haluat testata käytäntöä ensin testitilassa, katso [käytännön](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) käyttäminen testitilassa ja DLP-käytännön luominen, testaaminen [ja hienosäätäminen.](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy) 