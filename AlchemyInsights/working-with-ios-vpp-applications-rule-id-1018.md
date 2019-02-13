---
title: IOS VPP sovellusten säännön tunnus 1018 käsitteleminen
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29917493"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="6f2cc-102">IOS VPP-sovellusten käyttäminen</span><span class="sxs-lookup"><span data-stu-id="6f2cc-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="6f2cc-103">Lue lisätietoja toiminnot, rajoitukset ja toimenpiteet [iOS apps ostaa aseman osto - ohjelma on Microsoft Intune – hallinta](https://docs.microsoft.com/intune/vpp-apps-ios) Apple aseman osto-ohjelma ja tuki-Microsoft Intune hyödyntää.</span><span class="sxs-lookup"><span data-stu-id="6f2cc-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="6f2cc-104">**Ongelmista:** ”Oma käyttäjille osoitettuja iOS VPP app, mutta asennus epäonnistui”.</span><span class="sxs-lookup"><span data-stu-id="6f2cc-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="6f2cc-p101">Näin voi käydä, jos yhden VPP-tunnusta käytetään useita kannettavan laitteen hallinnan palveluntarjoajien kautta. Apple-VPP-tunnuksia voi käyttää vain yksi toimittaja. Jos käytit VPP-tunnuksen kanssa useita tarjoajia, Lataa uudelleen Intune tunnuksen.</span><span class="sxs-lookup"><span data-stu-id="6f2cc-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="6f2cc-p102">Asennus saattaa epäonnistua myös, jos asennusten kokonaismäärä ylitä käyttöoikeuksien määrää. Voit tarkastella käyttöoikeuksiasi käyttöraportteja, siirry **Intune Mobile apps** \> **App-käyttöoikeudet** -sivulla. Lisätietoja vapauttaa lisenssejä käyttää, on [Tässä artikkelissa.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="6f2cc-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

