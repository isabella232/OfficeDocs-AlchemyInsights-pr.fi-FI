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
ms.openlocfilehash: 5a285f36aeb814e3b1d361c8cbffd5a6bef0770d10082d24654c7bbda59ce65b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082183"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a>Tiettyihin Office 365 lähetettyjen sähköpostiviestien automaattinen salaaminen

1. Valitse [Exchange hallintakeskuksessa](https://outlook.office365.com/ecp/) **Postinkulku > säännöt**. 
2. Napsauta Uusi **(+) -kuvaketta** ja valitse sitten **Käytä Office 365 -salaus viestien suojausta.**
3. Kirjoita Nimi-ruutuun säännön nimi, kuten *Salaa* contoso.com.
4. Valitse **Käytä tätä sääntöä, jos**-kohdassa > toimialue **on**. 
5. Kirjoita toimialueen nimi, kuten **contoso.com.**
6. Napsauta Lisää **(+) -kuvaketta** ja valitse sitten **OK**.
7. Valitse Tee **seuraava kenttä -kohdan** vierestä **Valitse yksi**. 
8. Valitse **RMS-mallin** avattavasta valikosta **Salaa** ja valitse sitten **OK**. (Jos et näe tätä vaihtoehtoa, se tarkoittaa, että suunnitelmasi ei sisällä automaattista salausta. Voit kuitenkin lisätä sen!)
9. Valitse mikä tahansa valinnainen valinta (luettelo valinnaisista valituksista, jotka voit tehdä tässä vaiheessa, joista monet voidaan jättää oletusarvoon yksinkertaisuuden vuoksi).
10. Valitse **Tallenna**.

> [!IMPORTANT]
> Voit aina palata takaisin ja muokata tätä sääntöä myöhemmin.

Lisätietoja salauksen sääntöjen luomisesta on kohdassa Sähköpostin kulkusääntöjen [määrittäminen sähköpostiviestien salaamiseen Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)