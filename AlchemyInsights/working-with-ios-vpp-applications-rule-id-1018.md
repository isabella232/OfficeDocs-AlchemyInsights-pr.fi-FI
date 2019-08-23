---
title: IOS VPP sovellusten säännön tunnus 1018 käsitteleminen
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: a0bbc1f49f251ef4f16300c8cca98e219008d17e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/22/2019
ms.locfileid: "36557989"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="1c625-102">IOS VPP-sovellusten käyttäminen</span><span class="sxs-lookup"><span data-stu-id="1c625-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="1c625-103">Lue lisätietoja toiminnot, rajoitukset ja toimenpiteet [iOS apps ostaa aseman osto - ohjelma on Microsoft Intune – hallinta](https://docs.microsoft.com/intune/vpp-apps-ios) Apple aseman osto-ohjelma ja tuki-Microsoft Intune hyödyntää.</span><span class="sxs-lookup"><span data-stu-id="1c625-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="1c625-104">**Ongelmista:** ”Oma käyttäjille osoitettuja iOS VPP app, mutta asennus epäonnistui”.</span><span class="sxs-lookup"><span data-stu-id="1c625-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="1c625-105">Näin voi käydä, jos yhden VPP-tunnusta käytetään useita kannettavan laitteen hallinnan palveluntarjoajien kautta.</span><span class="sxs-lookup"><span data-stu-id="1c625-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="1c625-106">Apple-VPP-tunnuksia voi käyttää vain yksi toimittaja.</span><span class="sxs-lookup"><span data-stu-id="1c625-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="1c625-107">Jos käytit VPP-tunnuksen kanssa useita tarjoajia, Lataa uudelleen Intune tunnuksen.</span><span class="sxs-lookup"><span data-stu-id="1c625-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="1c625-108">Asennus saattaa epäonnistua myös, jos asennusten kokonaismäärä ylitä käyttöoikeuksien määrää.</span><span class="sxs-lookup"><span data-stu-id="1c625-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="1c625-109">Voit tarkastella käyttöoikeuksiasi käyttöraportteja, siirry **Intune Mobile apps** \> **App-käyttöoikeudet** -sivulla.</span><span class="sxs-lookup"><span data-stu-id="1c625-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="1c625-110">Lisätietoja vapauttaa lisenssejä käyttää, on [Tässä artikkelissa.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="1c625-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
