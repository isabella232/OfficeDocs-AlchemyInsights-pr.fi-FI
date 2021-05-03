---
title: Ongelmia SharePoint Windows 7-koneissa
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/28/2021
ms.locfileid: "52125118"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a><span data-ttu-id="21d7e-102">Ongelmia SharePoint Windows 7-koneissa</span><span class="sxs-lookup"><span data-stu-id="21d7e-102">Issues with SharePoint on Windows 7 machines</span></span>

<span data-ttu-id="21d7e-103">Jos saat virheitä Windows 7 -koneissa SharePoint OneDrive, ne voivat olla liittyviä TLS 1.0/1.1 -käyttöympäristön jämähtämiseen.</span><span class="sxs-lookup"><span data-stu-id="21d7e-103">If you receive errors on Windows 7 machines while working on SharePoint or OneDrive, they might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="21d7e-104">Lisätietoja on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="21d7e-104">For more information, see:</span></span>

- [<span data-ttu-id="21d7e-105">TLS 1.2:n valmistelu Office 365:ssä ja Office 365 GCC:ssä</span><span class="sxs-lookup"><span data-stu-id="21d7e-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- <span data-ttu-id="21d7e-106">Windows 7 SP1/Windows 8 -asiakasasiakkaissa on oltava TLS1.2 käytössä.</span><span class="sxs-lookup"><span data-stu-id="21d7e-106">Windows 7 SP1/Windows 8 clients must have TLS1.2 enabled.</span></span> <span data-ttu-id="21d7e-107">Lisätietoja on kohdassa [Todennusvirheitä ilmenee, kun asiakasohjelmalla ei ole TLS 1.2 -tukea](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span><span class="sxs-lookup"><span data-stu-id="21d7e-107">For more information, see [Authentication errors occur when client doesn't have TLS 1.2 support](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span></span>

- <span data-ttu-id="21d7e-108">Asenna KB3140245 ja luo rekisteriarvo.</span><span class="sxs-lookup"><span data-stu-id="21d7e-108">Install KB3140245 and create the registry value.</span></span> <span data-ttu-id="21d7e-109">Lisätietoja on WinHTTP in Windows -sovelluksen päivityksessä [TLS 1.1: n ja TLS 1.2:n](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) käyttöönottamiseksi Windows</span><span class="sxs-lookup"><span data-stu-id="21d7e-109">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)</span></span>

- <span data-ttu-id="21d7e-110">Windows 7 SP1/Windows 8-asiakkaiden on varmistettava, että uusimmat TLS-salauspaketit on asennettu.</span><span class="sxs-lookup"><span data-stu-id="21d7e-110">Windows 7 SP1/Windows 8 clients must ensure latest TLS cipher suites are installed.</span></span> <span data-ttu-id="21d7e-111">Lisätietoja on kohdassa [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058).</span><span class="sxs-lookup"><span data-stu-id="21d7e-111">For more information, see [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058).</span></span> 


