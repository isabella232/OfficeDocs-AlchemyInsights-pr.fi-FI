---
title: Salasanan synkronointiin liittyviä ongelmia
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387874"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="f061c-102">Salasanan synkronointiin liittyviä ongelmia</span><span class="sxs-lookup"><span data-stu-id="f061c-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="f061c-103">Voit tehdä salasanojen synkronointiongelmien vianmäärityksen käynnistämällä tämän AAD Connect -vianmääritystehtävän avulla, miksi salasanoja ei synkronoida.</span><span class="sxs-lookup"><span data-stu-id="f061c-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="f061c-104">Aloita siirtymällä [kohtaan Suoran synkronoinnin hallinta](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="f061c-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="f061c-105">Avaa uusi Windows PowerShell -istunto Azure AD Connect -palvelimessa ja valitse **Suorita järjestelmänvalvojana** -vaihtoehto.</span><span class="sxs-lookup"><span data-stu-id="f061c-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="f061c-106">Suorita Set-ExecutionPolicy RemoteSigned tai Set-ExecutionPolicy Unrestricted.</span><span class="sxs-lookup"><span data-stu-id="f061c-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="f061c-107">Käynnistä ohjattu Azure AD Connect -toiminto.</span><span class="sxs-lookup"><span data-stu-id="f061c-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="f061c-108">Siirry Lisätehtävät-sivulle > **Seuraava - vianmääritys**  >  **Next**.</span><span class="sxs-lookup"><span data-stu-id="f061c-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="f061c-109">Avaa PowerShellin vianmääritysvalikko valitsemalla **Käynnistä.**</span><span class="sxs-lookup"><span data-stu-id="f061c-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="f061c-110">Valitse **Salasanan synkronoinnin vianmääritys**.</span><span class="sxs-lookup"><span data-stu-id="f061c-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="f061c-111">Ongelmana on yleensä se, että salasanaa ei synkronoida tietylle käyttäjätilille.</span><span class="sxs-lookup"><span data-stu-id="f061c-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="f061c-112">**Osan sisällöstä toimittaa** Salasanan synkronointi epäonnistuu, jos viimeinen onnistunut salasanan synkronointi oli jokin aika sitten.</span><span class="sxs-lookup"><span data-stu-id="f061c-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="f061c-113">Lisätietoja salasanojen synkronoinnin vianmäärityksestä on [ohjeaiheessa Salasanan hajautussynkronoinnin vianmääritys Azure AD Connect -synkronoinnin kanssa](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="f061c-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>