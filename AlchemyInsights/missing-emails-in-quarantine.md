---
title: Puuttuvia sähköpostiviestejä karanteenissa
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 563f76f624f428a46894268b478cf05eb757b497
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539821"
---
# <a name="missing-emails-in-quarantine"></a>Puuttuvia sähköpostiviestejä karanteenissa"

Järjestelmänvalvojat [voivat tarkastella, vapauttaa tai poistaa näitä viestejä.](/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files)

Avaa Tietoturva- &- ja yhteensopivuuskeskus osoitteessa [https://protection.office.com](https://protection.office.com/) . Jos haluat avata Karanteeni-sivun suoraan, siirry [https://protection.office.com/quarantine](https://protection.office.com/quarantine) -sivulle.  

Voit hakea seuraavien arvojen perusteella:  

- **Viestitunnus:** viestin yleinen yksilöllinen tunniste. Jos valitset viestin luettelosta, Viestin  tunnus -arvo näkyy näyttöön tulevassa Tiedot-pikaikkunaruudussa.  Järjestelmänvalvojat voivat [viestien jäljityksen](/microsoft-365/security/office-365-security/message-trace-scc) avulla etsiä viestejä ja niiden vastaavia viestitunnusarvoja.
- **Lähettäjän sähköpostiosoite:** yksittäisen lähettäjän sähköpostiosoite.
- **Vastaanottajan sähköpostiosoite:** yksittäisen vastaanottajan sähköpostiosoite.
- **Aihe:** Käytä viestin koko aihetta. Kirjainko eri kirjainkooissa ei ole merkitystä haussa.

Kun olet antanut hakuehdot, suodata ![ tulokset valitsemalla ](/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  Päivitä-painike Päivitä.

Cmdlet-komennot, joita käytetään karanteeniin asetettujen viestien ja tiedostojen tarkastelemiseen ja hallintaan, ovat seuraavat:
- [Delete-QuarantineMessage](/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](/powershell/module/exchange/preview-quarantinemessage): Huomaa, että tämä cmdlet-komento on vain viesteille, ei haittaohjelmille, jotka ovat peräisin Microsoft Defender for Office 365 for SharePoint Onlinesta, OneDrive for Business tai Teams.
- [Release-QuarantineMessage](/powershell/module/exchange/release-quarantinemessage)