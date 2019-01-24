---
title: 1332 OWA - Saapuneet-kansion sääntöjen ei suoriteta postilaatikkoon
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f090d0a9d84bc6a4d1a1f4c0af55102d4b0ddfbe
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/24/2019
ms.locfileid: "29468081"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Saapuneet-sääntö ei toimi odotetulla tavalla

Tarkista seuraavat asetukset:
  
- Sanoma voidaan uudellenohjata, välitettyjen ja vastattujen automaattisesti Saapuneet-kansion sääntöjen perusteella vain kerran. Uudelleenohjataan sääntö (Saapuneet-kansion sääntö tai sähköpostin virtaussäännön, tunnetaan myös nimellä liikenteen sääntö) voit lisätä enintään kymmenen välityksen vastaanottajien viestin. Lisätietoja [kirjauskansion, kuljetus- ja Saapuneet-kansion säännön rajat](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).
    
- Vaihtoehtoinen lokiin postilaatikon Saapuneet-kansion säännöt eivät toimi. Saat lisätietoja vaihtoehtoinen lokiin postilaatikon [Vaihtoehtoinen lokiin postilaatikon](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).
    
Voit korjata nämä ongelmat, katso [kt 2829319](https://support.microsoft.com/kb/2829319).
  
Jos edellä kuvatut ongelmat eivät käytä, suorita Saapuneet-kansion säännön diagnostisen raportin ennen ongelmasta Microsoft Support Eskaloi:
  
1. Avaa postilaatikon Outlook Web ja **asetukset** \> **asetukset** \> **Järjestä sähköposti** \> **Saapuneet-kansion sääntöjä**.
    
2. Valitse sivun alareunassa **Jos säännöt eivät toimi voit Diagnostiikkaraportin luominen napsauttamalla tätä**.
    

