---
title: Määritettä ja suodatusta koskevat ongelmat
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481365"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Määritettä ja suodatusta koskevat ongelmat

**Ongelma ristiriitaisten UPN-arvojen kanssa**

Workday to AD User Provisioning Workday to AD User Provisioning (Työpäivä) näyttää **virhesanoman HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique.** Toiminto epäonnistui, koska lisäykselle tai muokkaukselle annettu UPN-arvo ei ole yksilöllinen koko metsää. Virheen tiedot: **CONSTRAINT_ATT_TYPE - userPrincipalName.**

**UserPrincipalName-arvo,** jonka Työpäivä-yhdistin yrittää määrittää luodessaan AD-käyttäjätiliä, on jo ad-kohdetoimialueella. Tämä tarkoittaa, että joko (1) käyttäjä on jo olemassa ja käyttäjän vastaava tunnuksen tarkistus epäonnistui, tai (2) UPN-luontisääntö loi ristiriitaisen arvon.

Seuraavassa on ehdotettuja ratkaisuvaiheita:

Jos käyttäjä on jo olemassa ja vastaavan tunnuksen tarkistus ei onnistunut yhdistämaan Työpäivä-tiliä Active Directory -tiliin, tarkista, onko vastaavan tunnusmääritteen (yleensä **työntekijätunnus)** sekä Työpäivä- että AD-tunnuksella tarkka vastine. Jos heillä ei ole vastaavuustietoja, ne on korjattava. Jos esimerkiksi Työpäivä-kohdan Työntekijätunnus on 001052 ja AD-arvo on 1052, valmistelumoduuli ei linkitä kahta tiliä ja yrittää luoda jo olemassa olevan käyttäjän. Tässä tapauksessa voit muuttaa TYÖNTEKIJÄNTUNNUS-arvoa AD:ssä niin, että siihen sisällytetään etunollat, jotta siitä tulee 001052. 
Jos UPN-luomislauseke ei luo yksilöllistä arvoa, harkitse kopiointia poistamisfunktion **SelectUniqueValue** avulla yksilöllistä arvoa joka kerta.

**Työpäiväksi AD-käyttäjien valmistelu ei määritä hallinnoijan määritearvoa AD-käyttäjätilille**

Työpäivä-asetukseksi AD-käyttäjien valmistelutyö ei määritä **ESIMIEHEN** määritearvoa AD-käyttäjätileille. Kun tämä tapahtuu, on kaksi mahdollista skenaariota:

1. Työpäivä-päällikköä ei voi ratkaista vastaavaksi AD-käyttäjätiliksi, koska esimies ei ole laajuudessa.
2. Usean **AD-toimialueen** skenaariossa Työpäivä-päällikkö ei ole samassa toimialueessa kuin käyttäjä.

Yritä ratkaista ongelma seuraavasti:

1. Jos olet määrittänyt vaikutusalueen suodattimia, tarkista ensin, onko esimies laajuudessa ja että se täyttää vaikutusalueen lausekkeen. Jos esimies ei täytä vaikutusalueen suodatusta, muuta suodatinta niin, että myös esimies kuuluu valmistelutoiminnon piiriin.
2. Jos sinulla on useita AD-toimialueita, yhdistimellä on tunnettu rajoitus, joka rajoittaa toimialueidenvälisten hallintaviittausten ratkaisemista.

Lisätietoja työpäivän määrittämisestä automaattista valmistelua varten on opetusohjelmassa: Työpäivän määrittäminen [automaattista käyttäjien valmistelua varten.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)













