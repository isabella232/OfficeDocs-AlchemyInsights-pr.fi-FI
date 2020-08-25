---
title: Lähetä muodossa Microsoft 365-ryhmä
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871790"
---
# <a name="send-as-microsoft-365-group"></a>Lähetä muodossa Microsoft 365-ryhmä

Voit määrittää Lähetä muodossa-käyttö oikeudet, jos haluat sallia tiettyjen käyttäjien lähettää viestejä Microsoft 365-ryhmänä:  

1. Muodosta yhteys Exchange Online PowerShelliin.  

2. Suorita seuraava komento:  

    Add-RecipientPermission `<GroupName>` -trustee `<MailboxName>` -accessrights SendAs

Lisä tietoja on Ohje aiheessa [jäsenten lähettämisen salliminen tai lähettäminen ryhmän puolesta](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).