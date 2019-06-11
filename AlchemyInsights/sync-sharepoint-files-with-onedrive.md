---
title: SharePoint-tiedostojen synkronointi OneDrive-synkronointisovelluksen avulla
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 5/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 74b79efeb7e46d03dc55f46252d152cd13e66c84
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757807"
---
# <a name="sync-sharepoint-files-with-the-new-onedrive-sync-client"></a><span data-ttu-id="2b051-102">SharePoint-tiedostojen synkronointi OneDrive-synkronointisovelluksen avulla</span><span class="sxs-lookup"><span data-stu-id="2b051-102">Sync SharePoint files with the new OneDrive sync client</span></span>

<span data-ttu-id="2b051-103">Avaa Resurssienhallinnassa -komento avaa Resurssienhallinnan paikallisen esiintymän, jossa näkyy SharePoint-sivustoa isännöivän palvelimen kansiorakenne.</span><span class="sxs-lookup"><span data-stu-id="2b051-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="2b051-104">On kuitenkin suositeltavaa [synkronoida SharePoint-tiedostot uudella OneDrive-synkronointiohjelmalla](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a>, joka sisältää [Tiedostot pyydettäessä](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) -toiminnon, sillä se mahdollistaa tiedostojen paikallisen käytön ja tarjoaa parhaan suorituskyvyn.</span><span class="sxs-lookup"><span data-stu-id="2b051-104">This being said , we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="2b051-105">Jos päätät käyttää resurssienhallintanäkymää uuden synkronointiohjelman sijaan, varmista, että noudatat alla olevissa artikkeleissa annettuja ohjeita ja parhaita käytäntöjä.</span><span class="sxs-lookup"><span data-stu-id="2b051-105">If you chose to use explorer view instead of using the new sync client, ensure you follow the steps and best practices in the articles below.</span></span>

- [<span data-ttu-id="2b051-106">SharePoint Onlinen ongelmien vianmääritys Avaa Resurssienhallinnassa -komennon avulla</span><span class="sxs-lookup"><span data-stu-id="2b051-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- <span data-ttu-id="2b051-107">[Kirjastotiedostojen kopioiminen tai siirtäminen Avaa Resurssienhallinnassa -komennolla](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)</span><span class="sxs-lookup"><span data-stu-id="2b051-107">See [Video: Copy or move library files by using Open with Explorer](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2).</span></span>

<span data-ttu-id="2b051-108">Huomautus:  Avaa Resurssienhallinnassa -painike ei näy uudessa kirjastokäyttökokemuksessa.</span><span class="sxs-lookup"><span data-stu-id="2b051-108">Note:  The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="2b051-109">Napsauta oikean yläkulman avattavaa Näytä-valikkoa (avattavan valikon nimi muuttuu käyttämäsi näkymän mukaan) ja valitse sitten Näytä Resurssienhallinnassa.</span><span class="sxs-lookup"><span data-stu-id="2b051-109">Click the View drop-down in the upper right (the name of the drop-down changes depending on your current view), and then click View in File Explorer.</span></span>

 <span data-ttu-id="2b051-110">SharePointin Avaa Resurssienhallinnassa -toiminto käyttää ActiveX-komponentteja, joten sitä tuetaan vain Internet Explorer -versioissa 10 ja 11.</span><span class="sxs-lookup"><span data-stu-id="2b051-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="2b051-111">Avaa Resurssienhallinnassa -komento ei toimi Windowsissa Microsoft Edgessä, Google Chromessa tai Mozilla Firefoxissa eikä Mac-käyttöympäristössä.</span><span class="sxs-lookup"><span data-stu-id="2b051-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="2b051-112">Tämän vuoksi Resurssienhallintanäkymä-vaihtoehto voi näkyä harmaana.</span><span class="sxs-lookup"><span data-stu-id="2b051-112">Due to this reason, the Explorer View option may be grayed out.</span></span>

- <span data-ttu-id="2b051-113">[Miksi SharePoint-valintanauhan painikkeet eivät ole käytettävissä tai näkyvät harmaana?](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca)</span><span class="sxs-lookup"><span data-stu-id="2b051-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  
