---
title: Ulkoisten käyttäjien lisääminen jakelu ryhmään
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737870"
---
# <a name="add-external-users-to-a-distribution-group"></a>Ulkoisten käyttäjien lisääminen jakelu ryhmään

Ulkoisen yhteys tiedon lisääminen jakelu ryhmään (DG) on kaksivaiheinen prosessi:
  
1. Luo Sähkö posti yhteys henkilö ulkoiselle käyttäjälle:
    
    1. Siirry hallinta keskukseen, **käyttäjien** > [yhteys tiedot](https://admin.microsoft.com/adminportal/home#/Contact) -sivulle. 
    
    2. Valitse **Lisää yhteys henkilö**.
    
    3. Kirjoita yhteys henkilön tiedot ja valitse **Lisää**.
    
2. Lisää Sähkö posti yhteys henkilö PÄÄOSASTOOSI:
    
    1. Siirry hallinta keskukseen, **ryhmät** > [ryhmät](https://admin.microsoft.com/adminportal/home#/groups) -sivulle. 
    
    2. Etsi DG, johon haluat lisätä ulkoisen käyttäjän, ja valitse se avataksesi Muokkaa-valinta ikkunan.
    
    3. Valitse **jäsenet** -väli lehdestä **Näytä kaikki ja Hallitse jäseniä**. 
    
    4. Valitse **Lisää jäseniä**.
    
    5. Valitse edellisessä vaiheessa luomasi Sähkö posti yhteys henkilö ja valitse sitten **Tallenna**.
    
Jos seuraavat toimet ulkoisten käyttäjien ei voi lähettää sähkö posteja DG tai eivät saa sähkö posteja siitä, se voisi olla, että DG on merkitty sallimaan vain sähkö postit sisäisille käyttäjille. Voit tarkistaa tämän kokoonpanon ja korjata sen [noudattamalla ohjeita.](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)
  
 **Huom:** Näitä ohjeita ei sovelleta, jos ryhmäsi tyyppi on "Office 365 Group" eikä "jakelu ryhmä". Tällöin voit lisätä ulkoisen käyttäjän suoraan ryhmään Outlookista. Lisä tietoja Office 365-ryhmistä sekä ohjeet ulkoisten vieraiden lisäämisestä löytyvät [tästä artikkelista](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  