---
title: Virtuaalinen määritys AAD-toimialueen palvelujen kanssa
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885201"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>Virtuaalinen määritys AAD-toimialueen palvelujen kanssa

Virtuaalimäärityksessä AAD-toimialueen palveluissa on seuraavat vaiheet: 

1. Toimialueen kuntotarkistuksen tarkistaminen Azure-portaalissa https://aka.ms/aadds-health
2. NSG:n tarkistaminen sääntöjä, jotka estävät portit, jotka tarvitaan portaalin Azure AD -toimialueen palveluissa synkronoinnissa https://aka.ms/aadds-networking
3. Sen varmistaminen, että virtuaalinen verkostosi otetaan käyttöön samalla Azure-alueella kuin Azure AD -toimialueen palveluiden hallinnoimaa toimialuetta.
4. Sen varmistaminen, että sinulla ei ole olemassa toimialuetta, jolla on sama toimialuenimi käytettävissä virtuaaliverkossa.

Lisätietoja AAD-toimialueen palveluja tukevan Azure Virtual Networkin suunnittelusta on virtual [network consideration -palvelussa.](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations)

