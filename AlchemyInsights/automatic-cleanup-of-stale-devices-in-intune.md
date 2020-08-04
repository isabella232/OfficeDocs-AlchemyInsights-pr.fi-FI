---
title: Automaattinen puhdistus tunkkainen laitteiden Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554966"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Automaattinen puhdistus tunkkainen laitteiden Intune

Intune antaa admin jotta configure aikaväliväliväli 90 ja 270 days, jonka jälkeen tunkkainen laitteet poistetaan palvelusta. Tämä asetus on organisaation laajuinen ja kun aktivoitu, se tulee voimaan välittömästi. Laitteet, joita ei ole kuitattu Intune-palvelimeen asetuksen ylittäväksi ajaksi, poistetaan pysyvästi.

**Huomautus** Vain MDM-laiteobjektit ovat oikeutettuja tähän puhdistustoimintoon. EAS:lle jää vain laiteobjektit pois.

Lisätietoja siitä, milloin laite voidaan poistaa laitteen puhdistusasetuksen ja sen "tilan" perusteella:

Asetus: **Poista laitteet viimeisen sisäänkirjautumispäivän jälkeen: Kyllä (jokin arvo (N) määritettyinä päivinä)**

- Intune-palvelu poistaa laitteen määritettyinä päivinä sen jälkeen, kun se on viimeksi kirjautunut sisään, arvon (N) perusteella.

Asetus: **Poista laitteet viimeisen sisäänkirjautumispäivän jälkeen: Ei**

- 180 päivän kuluttua laitteen varmenteen vanhenemisen päättymisestä eikä sitä uusita, laite poistetaan.

**Huomautus** Molemmissa tapauksissa laite on rekisteröitävä onnistuneesti Intunessa. Rekisteröinti tapahtuu ensimmäisen laitetarkastuksen aikana Intune-palvelussa.

Jos laite rekisteröityy intuneen, mutta ei rekisteröi sitä, laite poistetaan 270 päivän kuluttua rekisteröitymisestä. (90 päivää, jos haluat merkitä laitteen kumotuksi, ja sitten vielä 180 päivää tietueen poistamiseen.)

Intune-konsolissa ei ole tällä hetkellä mekanismia laitteen sertifioinnin vanhenemispäivän määrittämiseksi millekään laitteelle.