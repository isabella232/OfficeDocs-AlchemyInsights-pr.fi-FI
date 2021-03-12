---
title: Tiettyihin toimialueihin lähetettyjen Office 365 -sähköpostiviestien automaattinen salaaminen
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746053"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Tiettyihin toimialueihin lähetettyjen Office 365 -sähköpostiviestien automaattinen salaaminen

1. Valitse [Exchange-hallintakeskuksessa](https://outlook.office365.com/ecp/) **postinkulku- > säännöt.** 
2. Napsauta Uusi **(+) -kuvaketta** ja valitse sitten Käytä **Office 365 -viestin salausta ja** viestien oikeuksia.
3. Kirjoita **Nimi-kenttään** säännön nimi, kuten Salaa *contoso.com.*
4. Valitse **Käytä tätä sääntöä -kohdassa** **Vastaanottaja, > toimialue on**. 
5. Kirjoita toimialueen nimi, kuten **contoso.com.**
6. Napsauta Lisää **(+) -kuvaketta** ja valitse **sitten OK.**
7. Valitse Tee **seuraava kenttä -kohdan** vierestä **Valitse yksi.** 
8. Valitse **rms-mallin** avattavasta valikosta **Salaa** ja valitse sitten **OK.** (Jos et näe tätä vaihtoehtoa, se tarkoittaa, että suunnitelmasi ei sisällä automaattista salausta. Voit kuitenkin lisätä sen.)
9. Valitse mikä tahansa valinnainen valinta (luettelosta valinnaisia valintoja, jotka voit tehdä tässä vaiheessa, joista monet voidaan jättää yksinkertaisuuden oletusasetuksella).
10. Valitse **Tallenna**.

> [!IMPORTANT]
> Voit aina palata takaisin ja muokata tätä sääntöä myöhemmin.

Lisätietoja salaussääntöjen luomisesta on ohjeaiheessa Postinkulkusääntöjen määrittäminen [sähköpostiviestien salaamiseen Office 365:ssä](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)