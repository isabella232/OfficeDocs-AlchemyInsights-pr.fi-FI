---
title: Office 365 Advanced Threat Protection (ATP) -suojausongelmien vianmääritys
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 99bc985f2d66693aca45f0833ab47c043acc1324
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766742"
---
# <a name="troubleshoot-issues-with-office-365-atp"></a>Office 365 ATP:hen liittyvien ongelmien vianmääritys

- **Huomaatko viiveet sähköpostiviestin toimittamisessa?** Kokeile käyttää ATP Safe Attachments -käytäntöjen dynaamista toimitusta -vaihtoehtoa. Näin vältetään sähköpostiviestien toimitusviiveet ja suojataan vastaanottajia haitallisilta tiedostoilta.
- **Haluatko ilmoittaa vääriä positiivisia tai vääriä negatiivisia negatiivisia?** Tämän linkin avulla voit lähettää tiedoston analyysia varten:[https://microsoft.com/wdsi/filesubmission](https://microsoft.com/wdsi/filesubmission)
- **Tiesitkö, että voit ottaa ATP Safe Links -suojauksen käyttöön organisaation henkilöiden välillä lähetetyille sähköpostiviesteille?** Toimi seuraavasti:
    1. Siirry https://protection.office.comkohtaan ja kirjaudu sisään.
    2. Siirry **Uhkien** > **hallintapolicy** > **Safe Links**.
    3. Muokkaa (tai lisää) käytäntöä **käytännöt, jotka koskevat tiettyjä vastaanottajia.**
    4. Valitse **Käytä turvallisia linkkejä organisaation sisällä lähetettyihin viesteihin**.
    5. Tallenna käytäntö ja anna muutosten kulkea datakeskuksen läpi noin 30 minuuttia.
- Lisätietoja ATP:n kanssa on ohjeaiheessa [Office 365 Advanced Threat Protection](https://docs.microsoft.com/office365/securitycompliance/office-365-atp).