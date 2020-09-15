---
title: IOS:n VPP-sovellus säännön tunnuksen 1018 käyttö
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688943"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="f56f8-102">IOS:n VPP-sovellusten käyttö</span><span class="sxs-lookup"><span data-stu-id="f56f8-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="f56f8-103">Lue [, miten voit hallita Microsoft Intunen kautta ostettuja iOS-sovelluksia](https://docs.microsoft.com/intune/vpp-apps-ios) , joiden avulla saat tietoa ominaisuuksista, rajoitteista ja vaiheista, joilla voit hyödyntää Apple-määrä osto ohjelmaa ja sitä tukevia tietoja Microsoft Intunella.</span><span class="sxs-lookup"><span data-stu-id="f56f8-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="f56f8-104">**Yleisiä ongelmia:** "Määritin käyttäjälleni iOS-VPP-sovelluksen, mutta asennus epäonnistui."</span><span class="sxs-lookup"><span data-stu-id="f56f8-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="f56f8-105">Näin voi käydä, jos yksittäinen VPP-tunnus on käytössä useissa mobiililaitteiden hallinta palveluissa.</span><span class="sxs-lookup"><span data-stu-id="f56f8-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="f56f8-106">Applen VPP-tunnuksia voi käyttää vain yhden palveluntarjoajan kanssa.</span><span class="sxs-lookup"><span data-stu-id="f56f8-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="f56f8-107">Jos käytit VPP-tunnusta useiden palveluntarjoajien kanssa, sinun on ladattava tunnus uudelleen Intuneen.</span><span class="sxs-lookup"><span data-stu-id="f56f8-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="f56f8-108">Asennus voi epäonnistua myös, jos asennusten kokonaismäärä ylittää käyttö oikeuksien luku määrän.</span><span class="sxs-lookup"><span data-stu-id="f56f8-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="f56f8-109">Jos haluat tarkastella käyttö oikeuksia, siirry **Intune-mobiilisovellusten** \> **sovelluksen käyttö oikeudet** -sivulle.</span><span class="sxs-lookup"><span data-stu-id="f56f8-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="f56f8-110">Katso lisä tietoja käyttö oikeuksien hankkimisesta käytöstä [tässä artikkelissa.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="f56f8-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
