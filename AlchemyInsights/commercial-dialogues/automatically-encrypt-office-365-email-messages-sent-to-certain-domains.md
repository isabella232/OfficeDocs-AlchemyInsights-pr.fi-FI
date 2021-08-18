---
title: Tiettyihin Office 365 lähetettyjen sähköpostiviestien automaattinen salaaminen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: d30535d8605fcbfa0ca73c262d8f8671d73234a4
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318845"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Tiettyihin Office 365 lähetettyjen sähköpostiviestien automaattinen salaaminen

1. Valitse [Exchange hallintakeskuksessa](https://outlook.office365.com/ecp/) **Postinkulku ja > säännöt**. 
2. Napsauta Uusi **(+) -kuvaketta** ja valitse sitten **Käytä Office 365 -salaus ja oikeussuojaa viesteihin**.
3. Kirjoita Nimi-ruutuun säännön nimi, kuten *Salaa* contoso.com.
4. Valitse **Käytä tätä sääntöä, jos** **-kohdassa > toimialue on**. 
5. Kirjoita toimialueen nimi, kuten **contoso.com.**
6. Napsauta Lisää **(+) -kuvaketta** ja valitse sitten **OK**.
7. Valitse Tee **seuraava -kentän** vierestä **Valitse yksi**. 
8. Valitse **RMS-mallin** avattavasta valikosta **Salaa** ja valitse sitten **OK**. (Jos et näe tätä vaihtoehtoa, se tarkoittaa, että suunnitelmasi ei sisällä automaattista salausta. Voit kuitenkin lisätä sen!)
9. Valitse mikä tahansa valinnainen valinta (luettelo valinnaisista valituksista, jotka voit tehdä tässä vaiheessa, joista monet voidaan jättää oletusarvoon yksinkertaisuuden vuoksi).
10. Valitse **Tallenna**.

**Tärkeää:** Voit aina palata takaisin ja muokata tätä sääntöä myöhemmin.

Lisätietoja salauksen sääntöjen luomisesta on kohdassa Sähköpostin kulkusääntöjen [määrittäminen sähköpostiviestien salaamiseen Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)