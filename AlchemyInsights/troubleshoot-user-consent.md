---
title: Käyttäjän suostumuksen vianmääritys
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901193"
---
# <a name="troubleshoot-user-consent"></a>Käyttäjän suostumuksen vianmääritys

1. Voit määrittää, miten loppukäyttäjät hyväksyvät sovellukset Azure-portaalin tai PowerShellin kautta. Lisätietoja [on käyttäjän suostumusasetuksissa.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings)
1. Järjestelmänvalvoja voi myös microsoft [Graph -ohjelmointirajapinnan](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) avulla myöntää suostumuksen delegoiduille käyttöoikeuksille yksittäisen käyttäjän puolesta. Lisätietoja on kohdassa [Käytön saaminen käyttäjän puolesta.](https://docs.microsoft.com/graph/auth-v2-user)
1. [Käyttäjän suostumusvirheet:](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)tässä artikkelissa käsitellään virheitä, joita sovelluksen suostumuksen antamisen aikana voi ilmetä. Jos suoritat vianmäärityksen odottamattomia suostumuskehotteita, jotka eivät sisällä virhesanomia, tutustu [Azure AD:n todennusskenaarioihin.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)