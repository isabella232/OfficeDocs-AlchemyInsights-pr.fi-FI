---
title: N/MIME Outlookin verkko versiossa
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772259"
---
# <a name="encrypt-email-messages-in-outlook"></a>Sähkö posti viestien salaaminen Outlookissa

Microsoft 365-viestin salaus on luotu Microsoft Azure Rights Managementiin (Azure RMS), joka on osa Azure Information Protectionin suojausta. Jos tilauksesi sisältää Azure Rights Management-tai Azure Information Protectionin, **sinun ei tarvitse tehdä mitään toimenpiteitä, jotta voit ottaa käyttöön tai aktivoida** oikeuksien hallinta palvelun manuaalisesti.

Asiakas palautteen perusteella emme enää voi ottaa käyttöön Exchange-sähkö postin kulku sääntöjä, jos haluat automaattisesti salata lähtevän sähkö postin, joka sisältää tietyntyyppiset luottamukselliset tiedot oletusarvoisesti vuokra ajassa. Sen sijaan annamme yksityiskohtaisia ohjeita siitä, miten voit tehdä sen itse. Lisä tietoja siitä, miten voit luoda luottamukselliset tiedot salaamalla siirto säännön, on [tässä artikkelissa](https://aka.ms/OmeEtr).

- Jos käytät Outlookia verkossa (aiemmin **OWA**): Kun kirjoitat Sähkö posti viestiä, valitse **Protect** in OWA. Tämä koskee Älä lähetä edelleen-oikeutta. Valitse **Muuta käyttö oikeutta** ja salaa viesti valitsemalla **salaa** .

- Jos käytät **Outlook-asiakas ohjelmaa**: Jos haluat lähettää salatun viestin Outlook 2013 tai 2016 tai Outlook 2016 for Mac, valitse **Asetukset**  >  **Permissions**ja valitse sitten haluamasi suojaus vaihtoehto.

- Jos haluat **salata automaattisesti kaikki** tietyille vastaanottajalle tai ulkoisille kumppaneille lähetetyt sähkö postit, sinun on luotava sähkö postin kulun siirto sääntö Exchange-hallinta keskuksessa. Yksityiskohtaiset ohjeet ovat [tässä tuki artikkelissa](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

