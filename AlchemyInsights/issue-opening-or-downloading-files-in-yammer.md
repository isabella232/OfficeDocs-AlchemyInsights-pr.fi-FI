---
title: Tiedostojen avaamiseen tai lataamiseen liittyvä ongelma Yammerissa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148250"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Tiedostojen avaamiseen tai lataamiseen liittyvä ongelma Yammerissa

Classic Yammer tukee useita vaihtoehtoja tiedostojen lataamiseen viesteihin ja ryhmiin. Verkon kokoonpanosta riippuen tiedostot ovat oletusarvoisesti tallennustilaa SharePointissa.

Uuden Yammerin tiedostovalitsin ei vielä tue kaikkia perinteisessä Yammerissa käytettävissä olevia vaihtoehtoja. Tuleva päivitys lisää lisäominaisuuksia. Lisätietoja on [ohjeaiheessa Tiedoston tai kuvan liittäminen Yammer-keskusteluviestiin](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Tiedoston avaaminen tai lataaminen ei onnistu**  

Tiedosto saattaa ladata Yammerin, mutta se voidaan linkittää myös SharePoint Onlinen tiedostoon. Vianmääritys edellyttää, että määrität ensin tiedoston sijainnin. Jos tiedosto on ladattu Yammeriin, sillä on *.yammer.com URL-osoite. Varmista, että tarvittavat URL-osoitteet ja IP-osoitteet poistetaan. Lisätietoja on blogikirjoituksessa [Yammerin kovakoodatut IP-osoitteet ei suositella](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Tarkista, voiko käyttäjä, joka on myös yleinen järjestelmänvalvoja, ladata tiedoston. Jos tiedosto on yksityinen, saatat joutua käyttämään yksityistä sisältötilaa. Lisätietoja on kohdassa [Yksityisen sisällön valvonta Yammerissa](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Yammer-verkkotason vieraat ja tiedostot SharePoint Onlinessa**  

[Yammerin verkkotason vieraat](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) eivät käytä Azure AD B2B:tä ja ovat Yammer-palvelun sisäisiä, joten he eivät voi käyttää SharePointiin tallennettuja Yammer-tiedostoja. Luo ulkoinen AAD B2B -käyttäjä, joka voi käyttää SharePoint Onlinen tiedostokirjastoja kyseisen käyttäjätiedon avulla. Lisätietoja Yammerin tulevasta Azure AD B2B -vierastuesta on kohdassa [Business-to-business (B2B) Vierastuki Yammer Preview'ssa - Asiakkaan käyttöehdot ja usein kysytyt kysymykset](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).