---
title: Toimialueen palvelun salasanojen hash-synkronointi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177492"
---
# <a name="password-hash-synchronization-for-domain-service"></a>Toimialueen palvelun salasanojen hash-synkronointi

**Jos Azure AD DS -esiintymä kehottaa sinua sallimaan salasanojen hash-synkronoinnin**

Kohtaat skenaarion, jossa käytät yhdistelmäympäristöä ja käyttäjät synkronoivat paikallisesta Azure Active Directory Domain Services (AD DS) -ympäristöstä. Tämä skenaario havaitaan huolimatta siitä, että sinulla on salasanojen hash-synkronointi paikallisesta AD DS:stä Azure AD -vuokraajaan.

**Syy**

Näin tapahtuu, koska Azure AD Connect ei oletusarvoisesti synkronoi vanhoja New Technology LAN Manager (NTLM) - ja Kerberos-salasanojen hasheita, joita Azure AD DS:ssä tarvitaan.

**Vaihtoehtoinen menetelmä** 

Sinun on määritettävä Azure AD Connect synkronoimaan NTLM- ja Kerberos-todennusta varten tarvittavat salasanojen hasheet.

Kun Azure AD Connect on määritetty, paikallinen tilin luonti tai salasanan vaihtotapahtuma synkronoi myös vanhan salasanan hasheet Azure AD:n kanssa. Lisätietoja tästä [on](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) täällä ja ohjeita salasanojen synkronoinnin käyttöönottoon Azure AD DS -yhdistelmäympäristöissä.