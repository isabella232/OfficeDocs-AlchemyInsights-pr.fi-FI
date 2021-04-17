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
ms.openlocfilehash: 43f9a1f03084bf9adab706b3f77eff1d1db888ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831731"
---
# <a name="missing-emails-in-quarantine"></a>Puuttuvia sähköpostiviestejä karanteenissa"

Järjestelmänvalvojat [voivat tarkastella, vapauttaa tai poistaa näitä viestejä.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Avaa Tietoturva- &- ja yhteensopivuuskeskus osoitteessa [https://protection.office.com](https://protection.office.com/) . Jos haluat avata Karanteeni-sivun suoraan, siirry [https://protection.office.com/quarantine](https://protection.office.com/quarantine) -sivulle.  

Voit hakea seuraavien arvojen perusteella:  

- **Viestitunnus:** viestin yleinen yksilöllinen tunniste. Jos valitset viestin luettelosta, Viestin  tunnus -arvo näkyy näyttöön tulevassa Tiedot-pikaikkunaruudussa.  Järjestelmänvalvojat voivat [viestien jäljityksen](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) avulla etsiä viestejä ja niiden vastaavia viestitunnusarvoja.
- **Lähettäjän sähköpostiosoite:** yksittäisen lähettäjän sähköpostiosoite.
- **Vastaanottajan sähköpostiosoite:** yksittäisen vastaanottajan sähköpostiosoite.
- **Aihe:** Käytä viestin koko aihetta. Kirjainko eri kirjainkooissa ei ole merkitystä haussa.

Kun olet antanut hakuehdot, suodata ![ tulokset valitsemalla ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  Päivitä-painike Päivitä.  

Cmdlet-komennot, joita käytetään karanteeniin asetettujen viestien ja tiedostojen tarkastelemiseen ja hallintaan, ovat seuraavat:
- [Delete-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Export-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Get-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Huomaa, että tämä cmdlet-komento on vain viesteille, ei haittaohjelmille, jotka ovat peräisin ATP:stä SharePoint Onlinessa, OneDrive for Businessissa tai Teamsissa.
- [Release-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)