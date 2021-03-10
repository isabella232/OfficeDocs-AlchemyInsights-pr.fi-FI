---
title: SAML-allekirjoitusvarmenteen ongelmien vianmääritys
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693420"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>SAML-allekirjoitusvarmenteen ongelmien vianmääritys

Voit ratkaista SAML-allekirjoitusvarmenneongelman noudattamalla seuraavia suositeltuja ohjeita:

1. Kun lisäät yrityssovelluksen, joka tukee SSO:tä, Azure luo varmenteen, jonka nimi on [SAML-allekirjoitusvarmenne.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications) Tämän varmenteen vanhentumispäivä on kolme vuotta. Jos haluat muuttaa varmenteen vanhentumispäivää, katso lisätietoja liittoutumisvarmenteen vanhenemispäivän mukauttamisesta ja sen uudesta [varmenteesta.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)
2. Azure allekirjoittaa sovelluksen pyytämät SAML-tunnukset tämän varmenteen avulla ja lähettää sen sovellukseen onnistuneen SSO:n käyttöä varten. Jotta tämä on valmis, lataa varmenne Azure-portaalista ja lähetä se sovelluksen toimittajalle SSO-prosessin viimeistelemiseksi.

Kun tämä prosessi on valmis, sovellus luottaa tähän varmenteeseen, ja sovellus hyväksyy kaikki tällä varmenteella allekirjoitetut SAML-tunnukset.

3. Jos tämä varmenne vanhenee, luo uusi varmenne, päivitä se sovelluksen toimittajalle ja tee siitä aktiivinen Azure-puolella. Lisätietoja on kohdassa Pian [vanhentuvan varmenteen uusiminen.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)

> [!NOTE]
> Jos varmenne vanhenee, käyttäjää ei estetä.

4. [Lisää sähköpostiosoite, jonka ilmoitukset](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) vastaanotetaan ennen nykyisen varmenteen vanhenemista.

> [!NOTE]
> Vaihe 4 on valinnainen vaihe.

5. Muuta sovelluksen SAML-varmenteen allekirjoitusasetuksia ja varmenteen allekirjoitusalgoritmia. Lisätietoja on kohdassa Varmenteen [allekirjoitusasetusten ja allekirjoitusalgoritmin muuttaminen.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)

