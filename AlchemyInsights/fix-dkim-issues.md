---
title: DKIM asennuksen korjaamista varten.
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765021"
---
# <a name="fix-dkim-setup-issues"></a>DKIM asennuksen korjaamista varten.

Jos ilmenee ongelmia mahdollistaa mukautetun toimialueen DKIM, tekemällä seuraavat toimet:

- Useimmat DKIM-asennuksen ongelmat liittyvät virheellinen DNS-tietueet. Tarkista DKIM CNAME-tietue (**ei** TXT-tietue) on muotoiltu oikein. Lisätietoja Katso tätä [aihetta](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Jälkeen voit luoda tai päivittää DNS palvelua toimialueen (yleensä toimialueen registrar), että DKIM DNS-tietueet, odottaa välitystä DNS-tietueet.

- Jos ei voi luoda DKIM-DNS tietueita admin Centerissä, voit korvata \<CustomDomain\> kanssa mukautetun toimialueen (esimerkiksi contoso.com) ja suorita tämä komento [Exchange Online-PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.
