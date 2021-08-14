---
title: DKIM:n asennusongelmiin asentaminen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 5a613321ed79e657350ec4d19b1f07ac0a091b227a8268c793a10edd9990d41f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945928"
---
# <a name="fix-dkim-setup-issues"></a>DKIM:n asennusongelmiin asentaminen

Jos DKIM:n käytössä mukautetussa toimialueessa ilmenee ongelmia, toimi seuraavasti:

- Useimmat DKIM:n määritysongelmat liittyvät virheellisiin DNS-tietueisiin. Tarkista, että DKIM CNAME -tietue **(ei** TXT-tietue) on muotoiltu oikein. Lisätietoja on tässä [ohjeaiheessa.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

- Kun olet luonut tai päivittänyt DKIM:n DNS-tietueet toimialueen DNS-isännöintipalvelussa (yleensä toimialuerekisteröijä), odota, että DNS-tietueet välittyvät.

- Jos et voi luoda DKIM DNS -tietueita hallintakeskuksessa, voit korvata mukautetun toimialueen (esimerkiksi contoso.com) ja suorittaa tämän komennon \<CustomDomain\> [Exchange Online PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .
