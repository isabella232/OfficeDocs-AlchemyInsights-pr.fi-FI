---
title: Sähkö postin välitys ongelmien korjaaminen sähkö postia käyttävänä julkisissa kansioissa
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366461"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>Sähkö postin välitys ongelmien korjaaminen sähkö postia käyttävänä julkisissa kansioissa

Jos ulkoiset lähettäjät eivät voi lähettää viestejä sähkö postia käyttäviin julkisiin kansioihin ja lähettäjät voivat saada virhe sanoman: **ei löytynyt (550 5.4.1)**, varmista, että yleisen kansion Sähkö posti toimi alue määritetään sisäisen välityksen toimi alueeksi hallitsevan toimi alueen sijaan:

1. Avaa [Exchange-hallinta keskus (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).

2. Siirry kohtaan **sähkö postin kulun** \> **hyväksytyt toimi alueet**, valitse hyväksytty toimi alue ja valitse sitten **Muokkaa**.

3. Valitse avautuvassa ominaisuudet-sivulla, jos toimi alueen tyypiksi on valittu **määräävä**, muuta arvoksi **sisäinen rele** ja sitten **Tallenna**.

Jos ulkoiset lähettäjät saavat virhe ilmoituksen, **sinulla ei ole käyttö oikeutta (550 5.7.13)**, voit tarkastella yleisen kansion anonyymien käyttäjien käyttö oikeuksia suorittamalla seuraavan komennon [Exchange Online PowerShellissä](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) :

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` Esimerkiksi `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .

Jos haluat, että ulkoiset käyttäjät voivat lähettää sähkö postia tähän julkiseen kansioon, lisää CreateItems-käyttö oikeus käyttäjälle anonyymi. Esimerkiksi `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.
