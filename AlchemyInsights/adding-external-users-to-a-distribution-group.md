---
title: Ulkoisten käyttäjien lisääminen jakeluryhmään
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 7dbc69bced9ca800d3f95081b77dda5e49662579
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/27/2020
ms.locfileid: "43910929"
---
# <a name="add-external-users-to-a-distribution-group"></a>Ulkoisten käyttäjien lisääminen jakeluryhmään

Ulkoisen yhteyshenkilön lisääminen jakeluryhmään on kaksivaiheinen prosessi:
  
1. Luo sähköpostiyhteystieto ulkoiselle käyttäjälle:
    
    1. Siirry hallintakeskuksessa **Käyttäjien** > [yhteystiedot -sivulle.](https://admin.microsoft.com/adminportal/home#/Contact) 
    
    2. Valitse **Lisää yhteystieto**.
    
    3. Kirjoita yhteyshenkilön tiedot ja valitse **Lisää**.
    
2. Lisää sähköpostiyhteystieto pääosastoosi:
    
    1. Siirry hallintakeskuksessa **Ryhmät ryhmät** > [-sivulle.](https://admin.microsoft.com/adminportal/home#/groups) 
    
    2. Etsi pääosasto, jolle haluat lisätä ulkoisen käyttäjän, ja avaa muokkausikkuna valitsemalla se.
    
    3. Valitse **Jäsenet-välilehdessä** **Näytä kaikki ja hallitse jäseniä**. 
    
    4. Valitse **Lisää jäseniä**.
    
    5. Valitse edellisessä vaiheessa luomasi sähköpostiyhteystieto ja valitse sitten **Tallenna**.
    
Jos ulkoiset käyttäjät eivät voi näiden vaiheiden jälkeen lähettää sähköposteja pääosastolle tai vastaanottaa siitä sähköposteja, voi olla, että pääosasto on merkitty sallimaan vain sisäisten käyttäjien sähköpostit. Voit tarkistaa tämän kokoonpanon ja korjata sen noudattamalla ohjeita [täällä](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Huomautus:** Nämä ohjeet eivät päde, jos ryhmän tyyppi on Jakeluryhmä-asetuksen sijasta Microsoft 365 -ryhmä. Jos näin on, voit lisätä ulkoisen käyttäjän suoraan ryhmään Outlookista. Tässä [artikkelissa](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)on yksityiskohtaisia tietoja Microsoft 365 Groupsin vieraista sekä ohjeet ulkoisten vieraiden lisäämiseen.
  