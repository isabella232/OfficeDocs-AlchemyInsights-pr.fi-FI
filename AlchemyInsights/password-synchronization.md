---
title: Salasanan synkronoiminen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481446"
---
# <a name="password-synchronization"></a><span data-ttu-id="6f928-102">Salasanan synkronoiminen</span><span class="sxs-lookup"><span data-stu-id="6f928-102">Password synchronization</span></span>

<span data-ttu-id="6f928-103">**Salasanojen hash-synkronointi ei toimi lainkaan**</span><span class="sxs-lookup"><span data-stu-id="6f928-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="6f928-104">Joitakin yleisiä ongelmia, joita asiakkaat kohtaavat, kun salasanojen hash-synkronointi ei toimi, ovat:</span><span class="sxs-lookup"><span data-stu-id="6f928-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="6f928-105">Azure AD Connectin paikallisen Active Directory -yhteyden muodostamiseen käyttämälle  Active Directory  -tilille ei myönnetä replikoida hakemistomuutoksia ja replikoida hakemistomuutoksia, joten kaikki salasanasynkronoinnin edellyttämät käyttöoikeudet on korjattava myöntämällä nämä käyttöoikeudet Active Directory -tilille.</span><span class="sxs-lookup"><span data-stu-id="6f928-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="6f928-106">Salasanojen hash-synkronointi poistetaan käytöstä, kun järjestelmänvalvoja  on vaihtanut User Sign-In -menetelmän salasanasynkronoinnista toiseen vaihtoehtoon, kuten liittounnin **AD FS:ään** ohjatussa Azure AD Connect -toiminnossa . Voit korjata ongelman ottamalla salasanojen **hash-synkronointitoiminnon** uudelleen käyttöön ohjatussa Azure AD Connect -toiminnossa.</span><span class="sxs-lookup"><span data-stu-id="6f928-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="6f928-107">Paikallisen Active Directoryn yhteysongelma.</span><span class="sxs-lookup"><span data-stu-id="6f928-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="6f928-108">Esimerkiksi jotkin toimialueen ohjauskoneet eivät ole Azure AD [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) Connectin käytettävissä, tai palomuuri estää vaaditut portit. Tämä on korjattava varmistamalla, että Azure AD Connect -palvelimen ja paikallisen Active Directoryn välinen yhteys toimii oikein.</span><span class="sxs-lookup"><span data-stu-id="6f928-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="6f928-109">Azure AD Connect -palvelin on parhaillaan valmistelutilassa, jolloin palvelin ei voi käyttää salasanojen sulkuja. Voit ratkaista ongelman noudattamalla osiossa [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)-synkronoinnin salasanojen synkronoinnin vianmääritys - Salasanoja ei synkronoida.</span><span class="sxs-lookup"><span data-stu-id="6f928-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="6f928-110">**Salasanojen hash-synkronointi ei toimi joillakin käyttäjillä**</span><span class="sxs-lookup"><span data-stu-id="6f928-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="6f928-111">Jos olet huomannut, että salasanan hash ei synkronoidu  käyttäjälle, voit tutkia ja ratkaista ongelman Azure AD Connectin vianmääritystehtävän avulla.</span><span class="sxs-lookup"><span data-stu-id="6f928-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="6f928-112">Suorita seuraavat tehtävät:</span><span class="sxs-lookup"><span data-stu-id="6f928-112">Perform the following tasks:</span></span>

    <span data-ttu-id="6f928-113">a.</span><span class="sxs-lookup"><span data-stu-id="6f928-113">a.</span></span> [<span data-ttu-id="6f928-114">Suorita vianmääritystehtävä ohjatussa toiminnossa</span><span class="sxs-lookup"><span data-stu-id="6f928-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="6f928-115">b.</span><span class="sxs-lookup"><span data-stu-id="6f928-115">b.</span></span> [<span data-ttu-id="6f928-116">Salasanan hash-synkronointiongelman tutkiminen tietyssä käytössä cmdlet-vianmäärityksen cmdlet-komentoa käyttämällä</span><span class="sxs-lookup"><span data-stu-id="6f928-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="6f928-117">Paikallisen Active Directory -käyttäjäobjektin on oltava käytössä käyttäjän on vaihdettava salasana **seuraavalla kirjautumisvaihtoehdolla.**</span><span class="sxs-lookup"><span data-stu-id="6f928-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="6f928-118">Kun tämä asetus on käytössä, käyttäjälle määritetään tilapäinen salasana, ja sinua pyydetään vaihtamaan salasana seuraavassa kirjautumisessa.</span><span class="sxs-lookup"><span data-stu-id="6f928-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="6f928-119">Azure AD Connect ei synkronoi tilapäisiä salasanoja Azure AD:n kanssa.</span><span class="sxs-lookup"><span data-stu-id="6f928-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="6f928-120">Voit ratkaista edellä mainitun ongelman jommankumman seuraavista tehtävistä:</span><span class="sxs-lookup"><span data-stu-id="6f928-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="6f928-121">Pyydä käyttäjää kirjautumaan paikalliseen sovellukseen (esimerkiksi Windows-työpöydälle) ja vaihtamaan salasana.</span><span class="sxs-lookup"><span data-stu-id="6f928-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="6f928-122">Uusi salasana synkronoidaan Azure AD:n kanssa.</span><span class="sxs-lookup"><span data-stu-id="6f928-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="6f928-123">Järjestelmänvalvoja voi päivittää käyttäjän salasanan ilman, että käyttäjän on vaihdettava salasana seuraavalla kirjautumista **varten,** ja jakamaan uusi salasana käyttäjän kanssa.</span><span class="sxs-lookup"><span data-stu-id="6f928-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="6f928-124">Paikallisen Active Directory -käyttäjän objektia ei **ole määritetty oikein objektisynkronointia** tai salasanasynkronointia varten.</span><span class="sxs-lookup"><span data-stu-id="6f928-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="6f928-125">Voit tehdä vianmäärityksen noudattamalla artikkelissa Salasanojen hash-synkronoinnin vianmääritys [Azure AD Connect -synkronoinnin kanssa annettuja ohjeita.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)</span><span class="sxs-lookup"><span data-stu-id="6f928-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







