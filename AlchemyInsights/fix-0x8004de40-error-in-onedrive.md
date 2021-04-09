---
title: OneDriven 0x8004de40-virheen korjaus
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649745"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="da232-102">OneDriven 0x8004de40-virheen korjaus</span><span class="sxs-lookup"><span data-stu-id="da232-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="da232-103">Jos käyttöjärjestelmäsi on Windows 7 ja saat tämän virheilmoituksen, [TLS 1.1- ja TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)-protokollat otetaan käyttöön Windows-käyttöjärjestelmän WinHTTP -käyttöjärjestelmän oletusarvoisen suojatun protokollan päivityksen avulla.</span><span class="sxs-lookup"><span data-stu-id="da232-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="da232-104">Jos käytössäsi on Windows 10 ja saat virheilmoituksen 0x8004de40 OneDrivesta:</span><span class="sxs-lookup"><span data-stu-id="da232-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="da232-105">Käynnistä tietokone uudelleen, kun yhteys Acitve-hakemistotoimialueeseen on muodostettu.</span><span class="sxs-lookup"><span data-stu-id="da232-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="da232-106">Jos uudelleenkäynnistys ei korjaa ongelmaa, poista laitteen kiinnitys ja lisää se uudelleen Azure AD:stä.</span><span class="sxs-lookup"><span data-stu-id="da232-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="da232-107">**Huomautus:** sinun pitäisi olla yrityksen verkossa, kun suoritat näitä vaiheita.</span><span class="sxs-lookup"><span data-stu-id="da232-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="da232-108">Älä suorita näitä vaiheita, kun et ole yhteydessä yrityksen infrastruktuuriin (esimerkiksi matkustaessasi).</span><span class="sxs-lookup"><span data-stu-id="da232-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="da232-109">Avaa järjestelmänvalvojan oikeuksin suoritettava **komentokehote valitsemalla Käynnistä**, napsauttamalla **komentokehotetta** hiiren kakkospainikkeella ja valitsemalla sitten **Suorita järjestelmänvalvojana**.</span><span class="sxs-lookup"><span data-stu-id="da232-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="da232-110">Kirjoita *dsregcmd /leave ja paina* **Enter-näppäintä.**</span><span class="sxs-lookup"><span data-stu-id="da232-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="da232-111">Kun olet valmis, kirjoita *dsregcmd /join ja paina* **Enter-näppäintä.**</span><span class="sxs-lookup"><span data-stu-id="da232-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="da232-112">Kun olet valmis, sulje komentokehote.</span><span class="sxs-lookup"><span data-stu-id="da232-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="da232-113">Käynnistä tietokone uudelleen ja kirjaudu OneDriveen.</span><span class="sxs-lookup"><span data-stu-id="da232-113">Reboot the computer, and log into OneDrive.</span></span>