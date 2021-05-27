---
title: Ediscovery-sovelluksen vianmääritys sisältää virheitä
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676148"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>Ediscovery-sovelluksen vianmääritys sisältää virheitä

Onko eDiscovery-pitoon liittyviä ongelmia? Seuraavassa on joitakin parhaita käytäntöjä, jotka kannattaa ottaa huomioon:

- Tarkista pitojakauman tila.  Jos tila **on Käytössä (Odottaa) tai** Ei käytössä **(Odottaa),** odota, että pitojakelu on valmis.
- Yhdistä eDiscovery-pitopäivitykset yhdeksi joukkopyynnöksi sen sijaan, että päivität käytännön toistuvasti kullekin tapahtumalle.
- Suorita Set-CaseHoldPolicy <policyname> -Yritä uudelleenjakamista Tietoturva- ja yhteensopivuuskeskuksen Powershellissä. Lisätietoja on Näyttöyhteys [powershellin tietoturva& hallintakeskuksessa.](/powershell/exchange/connect-to-scc-powershell)

Ohjeet näiden asetusten tarkistamiseen sekä eDiscovery-pitoongelmien lieventämiseen ja ratkaisemiseen liittyvät parhaat käytännöt ovat kohdassa [eDiscovery-pitovirheiden vianmääritys.](/microsoft-365/compliance/hold-distribution-errors)
Lisätietoja muiden yleisimmät eDiscovery-ongelmien vianmäärityksestä ovat kohdassa [eDiscovery-ongelmien tutkiminen, vianmääritys ja ratkaiseminen.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)
