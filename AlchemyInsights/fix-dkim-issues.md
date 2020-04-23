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
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717559"
---
# <a name="fix-dkim-setup-issues"></a>DKIM-asennusongelmien korjaaminen

Jos dkimin käyttöönotossa mukautetussa toimialueella ilmenee ongelmia, toimi seuraavasti:

- Useimmat DKIM-asennusongelmat liittyvät virheellisiin DNS-tietueisiin. Varmista, että DKIM CNAME -tietue **(ei** TXT-tietue) on muotoiltu oikein. Lisätietoja on tässä [ohjeaiheessa](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

- Kun olet luonut tai päivittänyt DKIM DNS -tietueet toimialueesi DNS-isännöintipalvelussa (yleensä toimialueen rekisteröintipalvelussa), odota DNS-tietueiden levittämistä.

- Jos et voi luoda DKIM DNS -tietueita hallintakeskuksessa, \<voit\> korvata CustomDomain-toimialueen mukautetulla toimialueella (esimerkiksi contoso.com) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`ja suorittaa tämän komennon Exchange Online [PowerShellissä:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).
