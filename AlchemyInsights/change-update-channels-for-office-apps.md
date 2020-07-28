---
title: Office-sovellusten päivityskanavien muuttaminen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1740"
- "9000140"
ms.openlocfilehash: 4939682a6ca95c4f5475ee6aedea48c9ce83df7f
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439387"
---
# <a name="change-update-channels-for-office-apps"></a>Office-sovellusten päivityskanavien muuttaminen

Jos haluat käyttää uusia Office-asennuksia, valitse haluamasi päivityskanava Office-ohjelmiston latausasetuksilla ja asenna office-sovellukset (tai asenna ne uudelleen). Lisätietoja on [ohjeaiheessa Ohjelmiston latausasetusten hallinta Office 365:ssä](https://docs.microsoft.com/deployoffice/manage-software-download-settings-office-365). 

**Huomautus** Office-ohjelmiston latausasetuksilla valittu päivityskanava koskee kaikkia käyttäjiä, jotka suorittavat uusia asennuksia O365-portaalin avulla. Lisätietoja on [ohjeaiheessa Microsoft 365:n tai Office 2019:n lataaminen ja asentaminen uudelleen PC- tai Mac-tietokoneeseen](https://support.microsoft.com/office/download-and-install-or-reinstall-microsoft-365-or-office-2019-on-a-pc-or-mac-4414eaaf-0478-48be-9c42-23adc4716658).   

Jos käytössä on Office-asennuksia, siirry toiseen päivityskanavaan Officen käyttöönottotyökalun (ODT) avulla:  

1. Lataa Office Deployment Tool -työkalun (setup.exe) uusin versio [Microsoft Download Centeristä](https://go.microsoft.com/fwlink/p/?LinkID=626065).
2. Määritä sen kanavan nimi, johon haluat vaihtaa. Lisätietoja on [ohjeaiheessa Officen käyttöönottotyökalun määritysasetukset](https://docs.microsoft.com/DeployOffice/configuration-options-for-the-office-2016-deployment-tool#channel-attribute-part-of-add-element).
3. Luo määritys-XML-tiedosto, joka määrittää kanavan nimen, esimerkiksi update.xml.  
    a. <Configuration>  
    b. <päivitykset **Channel="Kuukausittain"** />  
    c. </Configuration>
4. Siirry komentoriviltä kansioon, jossa setup.exe sijaitsee, ja suorita seuraava komento:  
    a. setup.exe /configure update.xml
5. Käynnistä Office-sovellus (kuten Excel) ja **File**valitse sitten  >  **Tiedostotili**. Valitse Tuotetiedot-osassa **Päivitä asetukset**  >  **päivitä nyt**.

Lisätietoja on [ohjeaiheessa Aiemmin luotujen Office-sovellusten päivityskanavien vaihtaminen](https://support.microsoft.com/help/3185078/how-to-switch-from-semi-annual-channel-to-monthly-channel). 

Määritä Päivitä kanava -asetus ryhmäkäytäntöobjektin avulla, jos haluat vaihtaa valitun käyttäjäryhmän päivityskanavia tai käyttää Configuration Manageria (SCCM). Lisätietoja on [ohjeaiheessa Microsoft 365 -sovellusten päivityskanavien yleiskatsaus](https://docs.microsoft.com/deployoffice/overview-update-channels#group-policy). Lisätietoja on ohjeissa [Office 365 ProPlus -kanavien hallinta IT-ammattilaisille](https://techcommunity.microsoft.com/t5/office-365-blog/how-to-manage-office-365-proplus-channels-for-it-pros/ba-p/795813) ja [Microsoft 365 -sovellusten päivitysten hallinta Microsoft Endpoint Configuration Managerin avulla](https://docs.microsoft.com/deployoffice/manage-microsoft-365-apps-updates-configuration-manager).