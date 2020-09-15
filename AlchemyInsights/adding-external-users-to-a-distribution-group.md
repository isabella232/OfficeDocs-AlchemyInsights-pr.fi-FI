---
title: Ulkopuolisten käyttäjien lisääminen jakeluun
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663510"
---
# <a name="add-external-users-to-a-distribution-group"></a>Lisää ulkoiset käyttäjät jako ryhmään

Ulkoisen yhteys henkilön lisääminen jakelu ryhmään (DG) on kaksivaiheinen prosessi:
  
1. Sähkö posti yhteys henkilön luominen ulkoiselle käyttäjälle:
    
    1. Siirry hallinta keskuksessa **käyttäjät**-  >  [yhteys henkilöt](https://admin.microsoft.com/adminportal/home#/Contact) -sivulle. 
    
    2. Valitse **Lisää yhteys tieto**.
    
    3. Kirjoita yhteys henkilön tiedot ja valitse **Lisää**.
    
2. Lisää Sähkö posti yhteys tieto PÄÄOSASTOOSI:
    
    1. Siirry hallinta keskuksessa **ryhmät**  >  [ryhmät](https://admin.microsoft.com/adminportal/home#/groups) -sivulle. 
    
    2. Etsi pääosasto, johon haluat lisätä ulkoiset käyttäjät, ja valitse se avataksesi Muokkaa-valinta ikkunan.
    
    3. Valitse **jäsenet** -väli lehdessä **Näytä kaikki ja Hallitse jäseniä**. 
    
    4. Valitse **Lisää jäseniä**.
    
    5. Valitse edellisessä vaiheessa luomasi Sähkö posti yhteys tieto ja valitse sitten **Tallenna**.
    
Jos ulkoiset käyttäjät eivät voi lähettää sähkö posti viestejä pääosastolle tai eivät saa siitä Sähkö posti viestejä noudattamalla näitä ohjeita, voi olla, että pääosasto on merkitty sallimaan vain sisäisten käyttäjien lähettämät sähkö postit. Voit tarkistaa tämän määrityksen ja korjata sen noudattamalla [tässä](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)annettuja ohjeita.
  
 **Huomautus:** Näitä ohjeita ei sovelleta, jos ryhmän tyyppi on "Microsoft 365-ryhmä" eikä "Distribution Group". Tässä tapa uksessa voit lisätä ulkoiset käyttäjät suoraan ryhmään Outlookista. [Tässä artikkelissa](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)on lisä tietoja Microsoft 365-ryhmistä sekä ohjeita siitä, miten ulkoiset vieraat lisätään.
  