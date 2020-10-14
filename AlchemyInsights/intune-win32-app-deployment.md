---
title: Intune Win32-sovelluksen käyttöönotto
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461795"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="8fc96-102">Intune Win32-sovelluksen käyttöönotto</span><span class="sxs-lookup"><span data-stu-id="8fc96-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="8fc96-103">Microsoft Intune mahdollistaa Win32-sovellukset, mukaan lukien mutta ei rajoittuen MSI ja. EXE on otettu käyttöön Windows 10-laitteissa.</span><span class="sxs-lookup"><span data-stu-id="8fc96-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="8fc96-104">Käytettävä käyttöönotto mekanismi edellyttää, että Intune-hallinta laajennus (IME) on käytettävissä kohde laitteessa.</span><span class="sxs-lookup"><span data-stu-id="8fc96-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="8fc96-105">IME asennetaan automaattisesti, koska se on kohdistettu PowerShell-komento sarjaan tai Win32-sovelluksen käyttöönottoon käyttäjälle tai laitteelle.</span><span class="sxs-lookup"><span data-stu-id="8fc96-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="8fc96-106">On myös olemassa joukko ennakko edellytyksiä, jotka on täytettävä, jotta voit ottaa käyttöön Win32-sovelluksia, jotka sisältävät:</span><span class="sxs-lookup"><span data-stu-id="8fc96-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="8fc96-107">Tuettuja käyttö ympäristöjä: Windows 10-versio 1607 tai uudempi (Enterprise, Pro ja Education-versiot).</span><span class="sxs-lookup"><span data-stu-id="8fc96-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="8fc96-108">Tuetuista arkkitehtuurista: x86 ja x64.</span><span class="sxs-lookup"><span data-stu-id="8fc96-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="8fc96-109">Laite hallinta: AAD liittyi ja automaattinen ilmoittautui (mukaan lukien yhdistelmä toimi alue liitetty ja ryhmä käytännön automaattinen kirjoittaja).</span><span class="sxs-lookup"><span data-stu-id="8fc96-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="8fc96-110">Sovellus paketin muoto:. [Microsoft Win32 Content prep-työkalun](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare)valmistelema **intunewin** -tiedosto.</span><span class="sxs-lookup"><span data-stu-id="8fc96-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="8fc96-111">Rajoitukset</span><span class="sxs-lookup"><span data-stu-id="8fc96-111">Limitations:</span></span>
    - <span data-ttu-id="8fc96-112">Enimmäiskoko: 8 gt.</span><span class="sxs-lookup"><span data-stu-id="8fc96-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="8fc96-113">Ei-tuettu arkkitehtuuri: aseet.</span><span class="sxs-lookup"><span data-stu-id="8fc96-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="8fc96-114">Tarkista asia kirja "[Microsoft Intune-sovelluksen lisää, Määritä ja valvo Win32-sovellus](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)"-kohdassa näitä vaiheita koskevia tietoja.</span><span class="sxs-lookup"><span data-stu-id="8fc96-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="8fc96-115">Tietoja sovelluksen käyttöönoton vian määrityksestä Windowsissa, mukaan lukien Win32-sovellukset, voi tarkistaa seuraavissa asia kirjoissa:</span><span class="sxs-lookup"><span data-stu-id="8fc96-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="8fc96-116">Sovelluksen asennus ongelmien vian määritys</span><span class="sxs-lookup"><span data-stu-id="8fc96-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="8fc96-117">Win32-sovellusten vian määritys</span><span class="sxs-lookup"><span data-stu-id="8fc96-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)