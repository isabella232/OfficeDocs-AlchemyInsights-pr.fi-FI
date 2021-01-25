---
title: Käyttäjän valmistelumääritteen yhdistäminen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949761"
---
# <a name="user-provisioning-attribute-mapping"></a>Käyttäjän valmistelumääritteen yhdistäminen

1. Lisätietoja tunnettujen määritteiden yhdistämisongelmien vianmäärityksestä on kohdassa [Määritteiden yhdistämismääritykset.](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings) 
2. Microsoft Azure Active Directory (AD) tukee käyttäjien valmistelua kolmannen osapuolen SaaS-sovelluksille, kuten Salesforcelle, G Suitelle ja muille. Jos otat käyttöön käyttäjän valmistelun kolmannen osapuolen SaaS-sovelluksessa, Azure-portaali ohjaa sen määritearvoja määritteiden yhdistämismääritysten avulla. Lisätietoja oletusmääritteiden yhdistämismääritysten mukauttamisesta on kohdassa Käyttäjän valmistelumääritteiden yhdistämismääritysten [mukauttaminen SaaS-sovelluksissa Azure Active Directoryssa.](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes)
    - Lisätietoja SaaS-sovelluksen käyttäjien valmistelusta on ohjeaiheessa Mikä on automaattinen [SaaS-sovelluksen käyttäjien valmistelu Azure AD:ssä?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. Kun mukautat määritteiden yhdistämismäärityksiä käyttäjän valmistelua varten, saatat nähdä, että määrite, jonka haluat yhdistää, ei näy Lähdemäärite-luettelossa. Synkronoi [määritteet](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) paikallisesta Active Directorysta Azure AD:n kanssa sovelluksen artikkeliin valmistelua varten. Näin voit lisätä puuttuvan määritteen synkronoimalla sen paikallisesta AD:stä Azure AD:lle.
