---
title: Vieraskäyttäjän ongelmien vianmääritys
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
- "9004358"
- "7822"
ms.openlocfilehash: 9e6030919721b4c0805a26ca45d365f31d88894e86ea08225f47576e7d152047
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939376"
---
# <a name="troubleshoot-guest-user-issues"></a>Vieraskäyttäjän ongelmien vianmääritys

1. Ohjeita sovellusten vieraskäyttöoikeuksien hallintaan on kohdassa Vieraskäyttöoikeuksien hallinta [Azure AD:n käyttöoikeussyistä.](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)
1. [Vieraskäyttäjien](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)lisääminen hakemistoon Azure-portaalissa: Tässä pika-aloitussivussa lisäät uuden vieraskäyttäjän Azure AD -hakemistoon Azure-portaalin kautta, lähetät kutsun ja näet, miltä vieraskäyttäjän kutsun lunastusprosessi näyttää.
1. [Vieraskäyttäjän lisääminen PowerShellin](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)avulla: Tässä pika-aloitustoiminnassa voit New-AzureADMSInvitation-komennolla yhden vieraskäyttäjän Azure-vuokraajaasi.
1. Lisätietoja käyttäjien ja ryhmien määrittämisestä yrityssovelluksiin Azure Active Directory:ssä (Azure AD:ssä) joko Azure-portaalista tai PowerShellin avulla on kohdassa Sovelluksen käyttäjämääritysten hallinta [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) 
1. Azure Active Directory (Azure AD) B2B -yhteistyö toimii useimpien Azure AD:n kanssa integroitujen sovellusten kanssa. Tässä artikkelissa [on](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)ohjeet suosittujen SaaS-sovellusten määrittämiseen Azure AD B2B:n kanssa käytettäväksi.
1. Organisaatiossa, joka Azure Active Directory (Azure AD) B2B -yhteistyöominaisuuksia kutsuaksesi vieraskäyttäjiä kumppaniorganisaatioista Azure AD:llesi, voit nyt tarjota näille B2B-käyttäjille pääsyn paikallisiin sovelluksiin. Nämä paikallisesti käytettävät sovellukset voivat käyttää SAML-pohjaista todennusta tai integroitua Windows -todennusta (IWA) Kerberosin rajoitettuun delegointiin (KCD). Lisätietoja on kohdassa Myönnä [Azure AD:n B2B-käyttäjille käyttöoikeudet paikallisiin sovelluksiin.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)
1. Lue, miten [voit myöntää paikallisesti hallittujen kumppanitilien käyttöoikeuden pilviresursseihin Azure AD B2B -yhteistyön avulla.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)