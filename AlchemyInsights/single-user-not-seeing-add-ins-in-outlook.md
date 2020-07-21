---
title: Yksittäinen käyttäjä ei näe apuosia Outlookissa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/16/2020
ms.locfileid: "45197834"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>Yksittäinen käyttäjä ei näe apuosia Outlookissa

Käyttäjä saattaa olla osa roolia, jolla ei ole oikeaa AppsForOfficeEnabled-parametria. Suorita tämä cmdlet-komento selvittääksesi, liittyykö oikea rooli käyttäjään:

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -delegointi $false | Format-Table -Automaattinen rooli,RoleAssigneeName,RoleAssigneeType

Lisätietoja on [ohjeaiheessa Outlookin apuohjelmia asennettavien ja hallitsevien järjestelmänvalvojien ja käyttäjien määrittäminen](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).
