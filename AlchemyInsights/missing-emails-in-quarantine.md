---
title: Puuttuvat sähkö postit karanteenissa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 55ed9a92675939c05477fbf6d12bbedd6eb931d6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673711"
---
# <a name="missing-emails-in-quarantine"></a>Puuttuvat sähkö postit karanteenissa "

Järjestelmänvalvojat voivat [tarkastella, vapauttaa tai poistaa näitä viestejä.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)

Jos haluat avata tieto turva & yhteensopivuus keskuksen, siirry [https://protection.office.com](https://protection.office.com/) . Jos haluat avata karanteeni sivun suoraan, siirry [https://protection.office.com/quarantine](https://protection.office.com/quarantine) .  

Voit hakea seuraavilla arvoilla:  

- **Viestin tunnus**: viestin yksilöivä tunnus. Jos valitset viestin luettelosta,  **viestin tunnuksen**  arvo näkyy näkyviin tulevassa  **tiedot**  -pikaruudussa. Järjestelmänvalvojat voivat etsiä viestejä ja niitä vastaavia viestin tunniste arvoja [viestin jäljityksen](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) avulla.
- **Lähettäjän Sähkö posti osoite**: yksittäisen lähettäjän Sähkö posti osoite.
- **Vastaanottajien Sähkö posti osoitteet**: yksi vastaanottajien Sähkö posti osoite.
- **Aihe**: Käytä viestin koko aihetta. Haussa kirjain koolla ei ole merkitsevä.

Kun olet lisännyt haku ehdot, ![ Suodata tulokset valitsemalla Päivitä-painike ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Päivitä** .  

Cmdlet-komennolla voit tarkastella ja hallita viestejä ja tiedostoja karanteenissa:
- [Poista-Karanteeninemessage](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [Vienti-Karanteeninemessage](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [Hanki-Karanteeninemessage](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- [Esikatselu-Quatarinemessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Huomaa, että tämä cmdlet on tarkoitettu vain viesteihin, ei Malware-tiedostoihin SharePoint Onlinen, OneDrive for Businessin tai teamsin kautta.
- [Tiedote-Karantiseinemessage](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)