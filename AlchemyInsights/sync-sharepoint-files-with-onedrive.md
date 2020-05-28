---
title: SharePoint Onlinen Avaa Resurssienhallinnassa -ongelmien määritys
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: be1136f7fd4575d482d38ee70163e5252d4ffbca
ms.sourcegitcommit: 5296874062b16f945d9a7a7a9ab29ec53686310b
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 05/21/2020
ms.locfileid: "44343174"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="e321f-102">SharePoint Onlinen Avaa Resurssienhallinnassa -ongelmien määritys</span><span class="sxs-lookup"><span data-stu-id="e321f-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="e321f-103">On suositeltavaa [synkronoida SharePoint-tiedostot uudella OneDrive-synkronointiohjelmalla](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88), joka sisältää [Tiedostot pyydettäessä](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) -toiminnon, sillä se mahdollistaa tiedostojen paikallisen käytön ja tarjoaa parhaan suorituskyvyn.</span><span class="sxs-lookup"><span data-stu-id="e321f-103">We recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>

<span data-ttu-id="e321f-104">Suorita Avaa Resurssienhallinnassa -ongelmien vianmääritys noudattamalla seuraavissa artikkeleissa annettuja ohjeita ja parhaita käytäntöjä:</span><span class="sxs-lookup"><span data-stu-id="e321f-104">To troubleshoot Open with Explorer issues, follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="e321f-105">SharePoint Onlinen ongelmien vianmääritys Avaa Resurssienhallinnassa -komennon avulla</span><span class="sxs-lookup"><span data-stu-id="e321f-105">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)
- [<span data-ttu-id="e321f-106">Kirjastotiedostojen kopioiminen tai siirtäminen Avaa Resurssienhallinnassa -komennolla</span><span class="sxs-lookup"><span data-stu-id="e321f-106">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

> <span data-ttu-id="e321f-107">**Huomautus:**</span><span class="sxs-lookup"><span data-stu-id="e321f-107">**Note:**</span></span>
>- <span data-ttu-id="e321f-108">Avaa Resurssienhallinnassa -komentoa tuetaan vain Internet Explorer 10:ssä tai 11:ssä.</span><span class="sxs-lookup"><span data-stu-id="e321f-108">Open with Explorer is only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="e321f-109">Avaa Resurssienhallinnassa -komento ei toimi Windowsissa Microsoft Edgessä, Google Chromessa tai Mozilla Firefoxissa eikä Mac-käyttöympäristössä.</span><span class="sxs-lookup"><span data-stu-id="e321f-109">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="e321f-110">Tämän vuoksi Resurssienhallintanäkymä-vaihtoehto voi näkyä harmaana.</span><span class="sxs-lookup"><span data-stu-id="e321f-110">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
>- <span data-ttu-id="e321f-111">Avaa Resurssienhallinnassa -painike ei näy uudessa kirjastokäyttökokemuksessa.</span><span class="sxs-lookup"><span data-stu-id="e321f-111">The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="e321f-112">Valitse oikean yläkulman avattava **Näytä**-valikko (avattavan valikon nimi muuttuu käyttämäsi näkymän mukaan) ja valitse sitten **Näytä Resurssienhallinnassa**.</span><span class="sxs-lookup"><span data-stu-id="e321f-112">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
