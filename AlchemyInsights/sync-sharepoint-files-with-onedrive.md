---
title: SharePoint Onlinen Avaa Resurssienhallinnassa -ongelmien määritys
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/7/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: afee367e250357b20b77f0ea5dfe66d68967eb2a
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270705"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="b318a-102">SharePoint Onlinen Avaa Resurssienhallinnassa -ongelmien määritys</span><span class="sxs-lookup"><span data-stu-id="b318a-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="b318a-103">Avaa Resurssienhallinnassa -komento avaa Resurssienhallinnan paikallisen esiintymän, jossa näkyy SharePoint-sivustoa isännöivän palvelimen kansiorakenne.</span><span class="sxs-lookup"><span data-stu-id="b318a-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="b318a-104">On kuitenkin suositeltavaa [synkronoida SharePoint-tiedostot uudella OneDrive-synkronointiohjelmalla](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a>, joka sisältää [Tiedostot pyydettäessä](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) -toiminnon, sillä se mahdollistaa tiedostojen paikallisen käytön ja tarjoaa parhaan suorituskyvyn.</span><span class="sxs-lookup"><span data-stu-id="b318a-104">This being said, we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="b318a-105">Jos päätät käyttää resurssienhallintanäkymää uuden OneDrive-synkronointiohjelman sijaan, varmista, että noudatat seuraavissa artikkeleissa annettuja ohjeita ja parhaita käytäntöjä:</span><span class="sxs-lookup"><span data-stu-id="b318a-105">If you chose to use Explorer view instead of using the new OneDrive sync client, make sure you follow the steps and best practices in the following articles:</span></span>

- [<span data-ttu-id="b318a-106">SharePoint Onlinen ongelmien vianmääritys Avaa Resurssienhallinnassa -komennon avulla</span><span class="sxs-lookup"><span data-stu-id="b318a-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- <span data-ttu-id="b318a-107">[Kirjastotiedostojen kopioiminen tai siirtäminen Avaa Resurssienhallinnassa -komennolla](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)</span><span class="sxs-lookup"><span data-stu-id="b318a-107">See [Video: Copy or move library files by using Open with Explorer](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2).</span></span>

> [!Note]  
> <span data-ttu-id="b318a-108">**Avaa Resurssienhallinnassa** -painike ei näy uudessa kirjastokäyttökokemuksessa.</span><span class="sxs-lookup"><span data-stu-id="b318a-108">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="b318a-109">Valitse oikean yläkulman avattava **Näytä**-valikko (avattavan valikon nimi muuttuu käyttämäsi näkymän mukaan) ja valitse sitten **Näytä Resurssienhallinnassa**.</span><span class="sxs-lookup"><span data-stu-id="b318a-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
>
 ><span data-ttu-id="b318a-110">SharePointin Avaa Resurssienhallinnassa -toiminto käyttää ActiveX-komponentteja, joten sitä tuetaan vain Internet Explorer -versioissa 10 ja 11.</span><span class="sxs-lookup"><span data-stu-id="b318a-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="b318a-111">Avaa Resurssienhallinnassa -komento ei toimi Windowsissa Microsoft Edgessä, Google Chromessa tai Mozilla Firefoxissa eikä Mac-käyttöympäristössä.</span><span class="sxs-lookup"><span data-stu-id="b318a-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="b318a-112">Tämän vuoksi Resurssienhallintanäkymä-vaihtoehto voi näkyä harmaana.</span><span class="sxs-lookup"><span data-stu-id="b318a-112">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
> - <span data-ttu-id="b318a-113">[Miksi SharePoint-valintanauhan painikkeet eivät ole käytettävissä tai näkyvät harmaana?](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca)</span><span class="sxs-lookup"><span data-stu-id="b318a-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

