---
title: DKIM-asennusongelmien korjaaminen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506771"
---
# <a name="fix-dkim-setup-issues"></a>DKIM-asennusongelmien korjaaminen

Jos sinulla on ongelmia DKIM:n käyttöönotossa mukautetussa toimialueessa, toimi seuraavasti:

- Useimmat DKIM:n asennusongelmat liittyvät virheellisiin DNS-tietueisiin. Varmista, että DKIM CNAME -tietue **(ei** TXT-tietue) on muotoiltu oikein. Lisätietoja on tässä [ohjeaiheessa](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

- Kun olet luonut tai päivittänyt DKIM DNS -tietueet toimialueesi DNS-isännöintipalvelussa (yleensä toimialueen rekisteröintipalvelussa), odota DNS-tietueiden levittämistä.

- Jos et voi luoda DKIM DNS -tietueita hallintakeskuksessa, voit korvata \<CustomDomain\> sen mukautetulla toimialueella (esimerkiksi contoso.com) ja suorittaa tämän komennon [Exchange Online PowerShellissä](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
