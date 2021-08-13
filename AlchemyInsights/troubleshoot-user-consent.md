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
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007895"
---
# <a name="troubleshoot-user-consent"></a>Käyttäjän suostumuksen vianmääritys

1. Voit määrittää, miten loppukäyttäjät suostuvat sovelluksiin Azure-portaalin tai PowerShellin kautta. Lisätietoja [on kohdassa Käyttäjän](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) suostumusasetukset.
1. Järjestelmänvalvoja voi myös [käyttää Microsoft Graph-ohjelmointirajapintaa](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) ja myöntää suostumuksen delegoiduille käyttöoikeuksille yksittäisen käyttäjän puolesta. Lisätietoja on kohdassa [Käytön saaminen käyttäjän puolesta.](https://docs.microsoft.com/graph/auth-v2-user)
1. [Käyttäjän suostumusvirheet:](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)tässä artikkelissa käsitellään virheitä, joita sovelluksen suostumuksen antamisen aikana voi ilmetä. Jos teet vianmäärityksessä odottamattomia suostumuskehotteita, jotka eivät sisällä virhesanomia, katso [Azure AD:n todennusskenaariot.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)