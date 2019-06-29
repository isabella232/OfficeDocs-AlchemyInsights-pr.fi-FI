---
title: 1332 OWA - Saapuneet-kansion sääntöjen ei suoriteta postilaatikkoon
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 7d1848830847fc6722da20e09a4875f49bf02bd3
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/28/2019
ms.locfileid: "35360914"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Saapuneet-sääntö ei toimi odotetulla tavalla

Tarkista seuraavat asetukset:

- Sanoma voidaan uudellenohjata, välitettyjen ja vastattujen automaattisesti Saapuneet-kansion sääntöjen perusteella vain kerran. Uudelleenohjataan sääntö (Saapuneet-kansion sääntö tai sähköpostin virtaussäännön, tunnetaan myös nimellä liikenteen sääntö) voit lisätä enintään kymmenen välityksen vastaanottajien viestin. Lisätietoja [kirjauskansion, kuljetus- ja Saapuneet-kansion säännön rajat](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Vaihtoehtoinen lokiin postilaatikon Saapuneet-kansion säännöt eivät toimi. Saat lisätietoja vaihtoehtoinen lokiin postilaatikon [Vaihtoehtoinen lokiin postilaatikon](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Voit korjata nämä ongelmat, katso [kt 2829319](https://support.microsoft.com/kb/2829319).

Jos edellä kuvatut ongelmat eivät käytä, suorita Saapuneet-kansion säännön diagnostisen raportin ennen ongelmasta Microsoft Support Eskaloi:

1. Avaa postilaatikon Outlook Web ja **asetukset** \> **asetukset** \> **Järjestä sähköposti** \> **Saapuneet-kansion sääntöjä**.

2. Valitse sivun alareunassa **Jos säännöt eivät toimi voit Diagnostiikkaraportin luominen napsauttamalla tätä**.
