---
title: Toimialueen palvelun salasanojen hash-synkronointi
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177492"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="b3ca7-102">Toimialueen palvelun salasanojen hash-synkronointi</span><span class="sxs-lookup"><span data-stu-id="b3ca7-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="b3ca7-103">**Jos Azure AD DS -esiintymä kehottaa sinua sallimaan salasanojen hash-synkronoinnin**</span><span class="sxs-lookup"><span data-stu-id="b3ca7-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="b3ca7-104">Kohtaat skenaarion, jossa käytät yhdistelmäympäristöä ja käyttäjät synkronoivat paikallisesta Azure Active Directory Domain Services (AD DS) -ympäristöstä.</span><span class="sxs-lookup"><span data-stu-id="b3ca7-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="b3ca7-105">Tämä skenaario havaitaan huolimatta siitä, että sinulla on salasanojen hash-synkronointi paikallisesta AD DS:stä Azure AD -vuokraajaan.</span><span class="sxs-lookup"><span data-stu-id="b3ca7-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="b3ca7-106">**Syy**</span><span class="sxs-lookup"><span data-stu-id="b3ca7-106">**Cause**</span></span>

<span data-ttu-id="b3ca7-107">Näin tapahtuu, koska Azure AD Connect ei oletusarvoisesti synkronoi vanhoja New Technology LAN Manager (NTLM) - ja Kerberos-salasanojen hasheita, joita Azure AD DS:ssä tarvitaan.</span><span class="sxs-lookup"><span data-stu-id="b3ca7-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="b3ca7-108">**Vaihtoehtoinen menetelmä**</span><span class="sxs-lookup"><span data-stu-id="b3ca7-108">**Workaround**</span></span> 

<span data-ttu-id="b3ca7-109">Sinun on määritettävä Azure AD Connect synkronoimaan NTLM- ja Kerberos-todennusta varten tarvittavat salasanojen hasheet.</span><span class="sxs-lookup"><span data-stu-id="b3ca7-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="b3ca7-110">Kun Azure AD Connect on määritetty, paikallinen tilin luonti tai salasanan vaihtotapahtuma synkronoi myös vanhan salasanan hasheet Azure AD:n kanssa.</span><span class="sxs-lookup"><span data-stu-id="b3ca7-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="b3ca7-111">Lisätietoja tästä [on](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) täällä ja ohjeita salasanojen synkronoinnin käyttöönottoon Azure AD DS -yhdistelmäympäristöissä.</span><span class="sxs-lookup"><span data-stu-id="b3ca7-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>