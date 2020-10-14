---
title: Intune Win32-sovelluksen käyttöönotto
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461795"
---
# <a name="intune-win32-app-deployment"></a>Intune Win32-sovelluksen käyttöönotto

Microsoft Intune mahdollistaa Win32-sovellukset, mukaan lukien mutta ei rajoittuen MSI ja. EXE on otettu käyttöön Windows 10-laitteissa. Käytettävä käyttöönotto mekanismi edellyttää, että Intune-hallinta laajennus (IME) on käytettävissä kohde laitteessa. IME asennetaan automaattisesti, koska se on kohdistettu PowerShell-komento sarjaan tai Win32-sovelluksen käyttöönottoon käyttäjälle tai laitteelle.

On myös olemassa joukko ennakko edellytyksiä, jotka on täytettävä, jotta voit ottaa käyttöön Win32-sovelluksia, jotka sisältävät:

- Tuettuja käyttö ympäristöjä: Windows 10-versio 1607 tai uudempi (Enterprise, Pro ja Education-versiot).
- Tuetuista arkkitehtuurista: x86 ja x64.
- Laite hallinta: AAD liittyi ja automaattinen ilmoittautui (mukaan lukien yhdistelmä toimi alue liitetty ja ryhmä käytännön automaattinen kirjoittaja).
- Sovellus paketin muoto:. [Microsoft Win32 Content prep-työkalun](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare)valmistelema **intunewin** -tiedosto.
- Rajoitukset
    - Enimmäiskoko: 8 gt.
    - Ei-tuettu arkkitehtuuri: aseet.

Tarkista asia kirja "[Microsoft Intune-sovelluksen lisää, Määritä ja valvo Win32-sovellus](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)"-kohdassa näitä vaiheita koskevia tietoja.

Tietoja sovelluksen käyttöönoton vian määrityksestä Windowsissa, mukaan lukien Win32-sovellukset, voi tarkistaa seuraavissa asia kirjoissa:

- [Sovelluksen asennus ongelmien vian määritys](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Win32-sovellusten vian määritys](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)