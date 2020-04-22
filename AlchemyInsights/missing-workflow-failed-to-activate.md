---
title: Puuttuva työnkulku ei onnistunut aktivoimaan
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 2598111005c219c398b63ca374e8e99348efc02c
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762098"
---
# <a name="missing-workflow-failed-to-activate"></a>Puuttuva työnkulku ei onnistunut aktivoimaan

Microsoft SharePoint -sivustokokoelmassa ei voi lisätä luetteloon tai kirjastoon yleisesti uudelleenkäytettävää työnkulkua (kuten Hyväksyntä - SharePoint 2010).
  
Voit ratkaista tämän ongelman seuraavasti: 
  
1. Avaa sivustokokoelman pääsivusto SharePoint Designer 2013:ssa.
  
2. Valitse **Sivustoobjektit**-kohdassa **Työnkulut**. 
  
3. Valitse **Työnkulut-valintanauhan** **Uusi-osassa** **Uudelleenkäytettävä työnkulku**. 
  
4. Kirjoita **Luo uudelleenkäytettävä työnkulku -lomakkeeseen** nimi ** *Repair2010* **. Valitse **Ympäristötyyppi**-kohdassa **SharePoint 2010 Workflow**ja valitse sitten **OK**. 
  
1. Valitse **Työnkulun** valintanauhan **Tallenna** -osassa **Julkaise**. 
  
2. Valitse **Työnkulku-valintanauhan** **Hallinta-osassa** **Julkaise yleisesti**. Valitse näyttöön tulevasta vahvistusvalintaikkunasta **OK**. 
  
3. Etsi web-selaimessa sivustokokoelman pääsivusto ja avaa **sivustoasetusten** \> **sivustokokoelman ominaisuudet**. Vaihda sitten **Työnkulut-ominaisuutta:** 
  
· Jos ominaisuus on *Aktivoitu* , valitse **Poista aktivointi** ja valitse sitten **Aktivoi**. 
  
· Jos toiminto on *poistettu käytöstä* , valitse **Aktivoi**. 
  
Lisätietoja on seuraavassa [artikkelissa](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

