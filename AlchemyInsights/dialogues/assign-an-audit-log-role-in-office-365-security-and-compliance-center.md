---
title: Valvontalokin roolin määrittäminen Office 365:n & yhteensopivuuskeskuksessa
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524791"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>Valvontalokin roolin määrittäminen Office 365:n & yhteensopivuuskeskuksessa

Office 365:n valvontalokista hakeminen edellyttää, että järjestelmänvalvojalle on  määritetty Vain tarkasteleminen -valvontalokien rooli tai Valvontalokit-rooli Exchange Onlinessa.  Nämä roolit määritetään oletusarvoisesti yhteensopivuuden hallinnan ja organisaation hallinnan rooliryhmille. Office 365:n ja Microsoft 365:n yleiset järjestelmänvalvojat lisätään automaattisesti Organisaation hallinta -rooliryhmän jäseniksi.

Jotta käyttäjä voi hakea mahdollisimman vähän käyttöoikeuksia, luo mukautettu rooliryhmä Exchange Onlinessa, lisää Vain  luku -valvontalokien rooli tai Valvontalokit-rooli ja lisää sitten käyttäjä uuden rooliryhmän jäseneksi. 

Lisätietoja on kohdassa Rooliryhmien [hallinta Exchange Onlinessa](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) ja valvontalokista hakeminen [tietoturva- & yhteensopivuuskeskuksessa.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)