---
title: Kaatuuko Teams?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030586"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="7c51d-102">Kaatuuko Teams?</span><span class="sxs-lookup"><span data-stu-id="7c51d-102">Teams client crashing?</span></span>

<span data-ttu-id="7c51d-103">Jos Teams-ohjelmasi kaatuu, kokeile seuraavia keinoja:</span><span class="sxs-lookup"><span data-stu-id="7c51d-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="7c51d-104">Jos käytät Teams-työpöytäsovellusta, varmista, että [sovellus on täysin ajan tasalla](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="7c51d-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="7c51d-105">Varmista, että kaikki [Office 365:n URL-osoitteet ja osoitealueet](https://docs.microsoft.com/microsoftteams/connectivity-issues) ovat käytettävissä.</span><span class="sxs-lookup"><span data-stu-id="7c51d-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="7c51d-106">Kirjaudu sisään järjestelmänvalvojatililläsi ja tarkista [palvelun kunnon koontinäytöstä](https://docs.microsoft.com/office365/enterprise/view-service-health), että palvelussa ei ole käyttökatkoja tai rajoituksia.</span><span class="sxs-lookup"><span data-stu-id="7c51d-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="7c51d-107">Viimeisenä keinona voit yrittää tyhjentää Teams-ohjelman välimuistin:</span><span class="sxs-lookup"><span data-stu-id="7c51d-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="7c51d-108">Sulje Microsoft Teams -työpöytäohjelma kokonaan.</span><span class="sxs-lookup"><span data-stu-id="7c51d-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="7c51d-109">Napsauta **Teamsia** hiiren kakkospainikkeella kuvakkeissa ja napsauta sitten **Lopeta**. Voit myös lopettaa prosessin täysin tehtävienhallinnassa.</span><span class="sxs-lookup"><span data-stu-id="7c51d-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="7c51d-110">Avaa Resurssienhallinta ja kirjoita %appdata%\Microsoft\teams.</span><span class="sxs-lookup"><span data-stu-id="7c51d-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="7c51d-111">Näet tässä hakemistossa seuraavia kansioita:</span><span class="sxs-lookup"><span data-stu-id="7c51d-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="7c51d-112">Siirry **Application Cache** -kansiossa Cache-alikansioon ja poista kaikki tiedostot tästä välimuistikansiosta:  %appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="7c51d-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="7c51d-113">Poista kaikki **Blob_storage**-kansion tiedostot: %appdata%\Microsoft\teams\blob_storage.</span><span class="sxs-lookup"><span data-stu-id="7c51d-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="7c51d-114">Poista kaikki **Cache**-kansion tiedostot: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="7c51d-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="7c51d-115">Poista kaikki **databases**-kansion tiedostot: %appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="7c51d-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="7c51d-116">Poista kaikki **GPUCache**-kansion tiedostot: %appdata%\Microsoft\teams\GPUCache.</span><span class="sxs-lookup"><span data-stu-id="7c51d-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="7c51d-117">Poista kaikki **IndexedDB**-kansion tiedostot: %appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="7c51d-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="7c51d-118">Poista kaikki **Local Storage** -kansion tiedostot: %appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="7c51d-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="7c51d-119">Poista vielä myös kaikki **tmp**-kansion tiedostot: %appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="7c51d-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="7c51d-120">Käynnistä Teams-ohjelma uudelleen.</span><span class="sxs-lookup"><span data-stu-id="7c51d-120">Restart your Teams client.</span></span>
