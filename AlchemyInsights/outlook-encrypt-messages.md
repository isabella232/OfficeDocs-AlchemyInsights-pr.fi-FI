---
title: S/MIME Outlookin verkkoversiossa
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511505"
---
# <a name="encrypt-email-messages-in-outlook"></a>Salaa sähköpostiviestit Outlookissa

Microsoft 365 -sanomien salaus perustuu Azure Information Protectioniin kuuluvaan Microsoft Azure Rights Managementiin (Azure RMS). Jos tilauksesi sisältää Azure Rights Managementin tai Azure Information Protectionin, sinun ei tarvitse tehdä mitään toimia oikeuksien hallintapalvelun **manuaaliseen käyttöönottoon tai aktivoimiseen.**

Asiakaspalautteen perusteella exchange-sähköpostin kulkusäännöt eivät enää anna Exchange-sähköpostin kulusääntöjä salata automaattisesti lähteviä sähköpostiviestejä, jotka sisältävät oletusarvoisesti tietyntyyppisiä arkaluonteisia tietoja vuokraajassasi. Sen sijaan annamme yksityiskohtaisia ohjeita siitä, miten voitte tehdä niin itse. Lisätietoja siirtosäännön luomisesta arkaluonteisten tietojen salaamista varten on [tässä artikkelissa](https://aka.ms/OmeEtr).

- Jos käytät Outlookin verkkoversiota (aiemmin **OWA):** Kun kirjoitat sähköpostiviestiä, valitse **Suojaa** OWA:ssa. Tämä koskee Älä välitä -oikeutta. Valitse **Muuta käyttöoikeuksia** ja valitse **Salaa,** jos haluat salata vain viestin.

- Jos käytät **Outlook-asiakasohjelmaa:** Jos haluat lähettää salatun viestin Outlook 2013:sta tai 2016:sta tai Outlook 2016 for Macista, valitse **Asetukset**  >  **Käyttöoikeudet**ja valitse sitten haluamasi suojausvaihtoehto.

- Jos haluat **salata automaattisesti kaikki** tietyille vastaanottajille tai ulkoisille kumppaniorganisaatioille lähetetyt sähköpostiviestit, sinun on luotava sähköpostin kulkua koskevan siirtosäännön Exchange-hallintakeskuksessa. Yksityiskohtaiset ohjeet ovat [tässä tukiartikkelissa](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).

