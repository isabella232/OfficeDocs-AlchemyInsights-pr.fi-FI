---
title: Microsoft Edgen muokkaaminen käyttämällä tieto hakemisto muuttujia kovakoodattu-polkujen sijaan
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 5c40aa1d7f61fbd2842839a5839899af8ab439f2
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/09/2020
ms.locfileid: "49677990"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>Microsoft Edgen muokkaaminen käyttämällä tieto hakemisto muuttujia kovakoodattu-polkujen sijaan

Esimerkiksi Windowsissa voit tallentaa profiili tiedot käyttäjän paikallisten sovellus tietojen alle oletus sijainnin sijaan määrittämällä **Userdatadir** -käytännöksi **$ {local_app_data} \edge\profile**. 

Lisä tietoja on artikkelissa [Microsoft Edge User Data-hakemiston muuttujien luominen](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars).