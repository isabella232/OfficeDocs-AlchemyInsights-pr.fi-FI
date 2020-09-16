---
title: Ratkaisuja Officen asentamiseen Terminal Serveriin liittyviin ongelmiin
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 85f24284-af6f-4624-b6be-901a4a9206eb
ms.openlocfilehash: df1a50031196fbd79662cee620fc41c7be14e179
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47738454"
---
# <a name="solutions-for-issues-around-installing-office-on-a-terminal-server"></a><span data-ttu-id="6f78b-102">Ratkaisuja Officen asentamiseen Terminal Serveriin liittyviin ongelmiin</span><span class="sxs-lookup"><span data-stu-id="6f78b-102">Solutions for issues around installing office on a Terminal Server</span></span>

<span data-ttu-id="6f78b-103">Jos haluat käyttää yhteiskäytössä olevaa tieto koneen Akti vointia, sinulla on oltava Microsoft 365-sovellusten Enterprise-version sisältävä tilaus.</span><span class="sxs-lookup"><span data-stu-id="6f78b-103">To use shared computer activation, you must have a subscription that includes Microsoft 365 Apps for enterprise.</span></span>
  
- <span data-ttu-id="6f78b-104">Varmista, että jaettujen tieto koneiden Akti vointi on otettu käyttöön</span><span class="sxs-lookup"><span data-stu-id="6f78b-104">Verify that shared computer activation is enabled</span></span>
- <span data-ttu-id="6f78b-105">Akti voinnin onnistumisen varmistaminen</span><span class="sxs-lookup"><span data-stu-id="6f78b-105">Verify that activation succeeded</span></span>
- <span data-ttu-id="6f78b-106">Jaetussa tieto koneessa tapahtuvan Akti voinnin virhe sanomien tarkasteleminen:</span><span class="sxs-lookup"><span data-stu-id="6f78b-106">Review error messages for shared computer activation:</span></span>
- <span data-ttu-id="6f78b-107">"Tililläsi löydettyjä tuotteita ei voi käyttää Officen aktivoimiseen jaetussa tieto kone skenaarioissa"</span><span class="sxs-lookup"><span data-stu-id="6f78b-107">"The products we found in your account cannot be used to activate Office in shared computer scenarios"</span></span>
  
<span data-ttu-id="6f78b-108">Tämä virhe tarkoittaa, että sinulla ei ole pakettia, joka sisältää Microsoft 365-sovelluksia yritykselle.</span><span class="sxs-lookup"><span data-stu-id="6f78b-108">This error means that you don't have a subscription that includes Microsoft 365 Apps for enterprise.</span></span>

<span data-ttu-id="6f78b-109">"Käyttöoikeudeton tuote"</span><span class="sxs-lookup"><span data-stu-id="6f78b-109">"Unlicensed Product"</span></span>

- <span data-ttu-id="6f78b-110">Tarkista, että käyttäjälle on määritetty Microsoft 365-sovellusten käyttö oikeus yritykselle.</span><span class="sxs-lookup"><span data-stu-id="6f78b-110">Check that the user is assigned a license for Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="6f78b-111">Tarkista, että käyttäjä kirjautuu käyttäjä tililleen.</span><span class="sxs-lookup"><span data-stu-id="6f78b-111">Check that the user signs in with their user account.</span></span>
- <span data-ttu-id="6f78b-112">Tarkista, että jaetussa tieto koneessa ja Inter netissä on yhteys.</span><span class="sxs-lookup"><span data-stu-id="6f78b-112">Check that there is connectivity between the shared computer and the Internet.</span></span>

<span data-ttu-id="6f78b-113">Lisä tietoja muista vian määritys vihjeistä on Ohje aiheessa [jaettujen tieto koneiden Akti voinnin ongelmien vian määritys](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="6f78b-113">For other troubleshooting tips, please see: [Troubleshoot issues with shared computer activation](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)</span></span>