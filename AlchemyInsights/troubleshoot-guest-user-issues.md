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
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901166"
---
# <a name="troubleshoot-guest-user-issues"></a>Vieraskäyttäjän ongelmien vianmääritys

1. Ohjeita sovellusten vieraskäyttöoikeuksien hallintaan on ohjeaiheessa Vieraskäyttö azure [AD](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)-käyttöoikeussyistä.
1. [Vieraskäyttäjien](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)lisääminen hakemistoon Azure-portaalissa: Tässä pika-aloitussivussa lisäät uuden vieraskäyttäjän Azure AD -hakemistoon Azure-portaalin kautta, lähetät kutsun ja näet, miltä vieraskäyttäjän kutsun lunastusprosessi näyttää.
1. [Lisää vieraskäyttäjä PowerShellin](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)avulla: Tässä pika-aloitustoiminnimessä voit New-AzureADMSInvitation yhden vieraskäyttäjän Azure-vuokraajaan.
1. Lisätietoja käyttäjien ja ryhmien määrittämisestä Azure Active Directoryn (Azure AD) yrityssovelluksiin joko Azure-portaalista tai PowerShellin avulla on ohjeaiheessa Sovelluksen käyttäjämäärityksen [hallinta Azure Active Directoryssa.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) 
1. Azure Active Directory (Azure AD) B2B -yhteistyö toimii useimpien Azure AD:n kanssa integroitujen sovellusten kanssa. Tässä artikkelissa [on](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)ohjeet suosittujen SaaS-sovellusten määrittämiseen Azure AD B2B:n kanssa käytettäväksi.
1. Organisaatiossa, joka käyttää Azure Active Directory (Azure AD) B2B -yhteistyöominaisuuksia kumppaniorganisaatioiden vieraskäyttäjien kutsumiseksi Azure AD:llesi, voit nyt tarjota näille B2B-käyttäjille pääsyn paikallisiin sovelluksiin. Näissä paikallisissa sovelluksissa voidaan käyttää SAML-pohjaista todentamista tai integroitua Windows-todennusta (IWA) Kerberosin rajoitettuun delegointiin (KCD). Lisätietoja on kohdassa [Azure AD:n B2B-käyttäjien](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)käyttöoikeuden myöntäminen paikallisiin sovelluksiin.
1. Lue, miten [voit myöntää paikallisesti hallittujen kumppanitilien käyttöoikeuden pilviresursseihin Azure AD B2B -yhteistyön avulla.](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)