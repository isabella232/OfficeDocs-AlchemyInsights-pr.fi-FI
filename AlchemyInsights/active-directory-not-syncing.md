---
title: Active Directory ei synkronoidu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697626"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="76152-102">Active Directory ei synkronoidu</span><span class="sxs-lookup"><span data-stu-id="76152-102">Active Directory not syncing</span></span>

<span data-ttu-id="76152-103">Jos saat synkronointi virheitä, kuten "ei hiljattain tehtyä synkronointia" tai huomaat, että Office-hallinta portaalin hakemisto synkronoinnin tilana lukee "synkronoitu viimeksi yli 3 päivää sitten", voi olla, että AADConnect-asetukset ovat virheelliset tai käyttö oikeudet eivät riitä synkronoinnin suorittamiseen.</span><span class="sxs-lookup"><span data-stu-id="76152-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="76152-104">AADConnect-toiminnon uudelleenasentaminen Pika-asetuksilla voi korjata ongelman nopeasti:</span><span class="sxs-lookup"><span data-stu-id="76152-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="76152-105">[Lataa AADConnect-tiedoston uusin versio](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="76152-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="76152-106">[Noudata pika-asennus ohjeita](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="76152-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="76152-107">Lisä tietoja AADConnect-palvelu tileiltä on Ohje aiheessa [Azure AD Connect: Asiakkaat ja käyttö oikeudet](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="76152-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
