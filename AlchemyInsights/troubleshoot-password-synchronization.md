---
title: Sala sanan synkronoinnin vian määritys
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664923"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="1cfce-102">Sala sanan synkronoinnin vian määritys</span><span class="sxs-lookup"><span data-stu-id="1cfce-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="1cfce-103">Voit määrittää Sala sanojen synkronointi ongelmien vian määrityksen käynnistämällä tämän AAD Connect-vian määritys tehtävän avulla, miksi Sala sanat eivät synkronoidu.</span><span class="sxs-lookup"><span data-stu-id="1cfce-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="1cfce-104">Aloita siirtymällä kohtaan [suoran synkronoinnin hallinta](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="1cfce-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="1cfce-105">Avaa uusi Windows PowerShell-istunto Azure AD Connect-palvelimessa ja valitse **Suorita järjestelmänvalvojana** -vaihto ehto.</span><span class="sxs-lookup"><span data-stu-id="1cfce-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="1cfce-106">Suorita sarja-ExecutionPolicy Remotsigned-tai ExecutionPolicy-käytäntönsä rajoittamattomat.</span><span class="sxs-lookup"><span data-stu-id="1cfce-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="1cfce-107">Käynnistä ohjattu Azure AD Connect-toiminto.</span><span class="sxs-lookup"><span data-stu-id="1cfce-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="1cfce-108">Siirry lisä tehtävät-sivulle > **vian määritys**  >  **Seuraava**.</span><span class="sxs-lookup"><span data-stu-id="1cfce-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="1cfce-109">Avaa PowerShellin vian määritys-valikko valitsemalla **Käynnistä** .</span><span class="sxs-lookup"><span data-stu-id="1cfce-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="1cfce-110">Valitse **Sala sanan synkronoinnin vian määritys**.</span><span class="sxs-lookup"><span data-stu-id="1cfce-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="1cfce-111">Ongelma on yleensä se, että tietyn käyttäjä tilin Sala sanaa ei synkronoida.</span><span class="sxs-lookup"><span data-stu-id="1cfce-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="1cfce-112">**Huomautukset** Sala sanojen synkronointi epäonnistuu, jos viimeinen onnistunut sala sana synkronoidaan jonkin aikaa sitten.</span><span class="sxs-lookup"><span data-stu-id="1cfce-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="1cfce-113">Lisä tietoja Sala sanan synkronoinnin vian määrityksestä on Ohje aiheessa [Sala sanan hajautus synkronoinnin vian määritys Azure AD Connect-synkronoinnin avulla](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="1cfce-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>