---
title: DKIM asennuksen korjaamista varten.
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765021"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="252e2-102">DKIM asennuksen korjaamista varten.</span><span class="sxs-lookup"><span data-stu-id="252e2-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="252e2-103">Jos ilmenee ongelmia mahdollistaa mukautetun toimialueen DKIM, tekemällä seuraavat toimet:</span><span class="sxs-lookup"><span data-stu-id="252e2-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="252e2-104">Useimmat DKIM-asennuksen ongelmat liittyvät virheellinen DNS-tietueet.</span><span class="sxs-lookup"><span data-stu-id="252e2-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="252e2-105">Tarkista DKIM CNAME-tietue (**ei** TXT-tietue) on muotoiltu oikein.</span><span class="sxs-lookup"><span data-stu-id="252e2-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="252e2-106">Lisätietoja Katso tätä [aihetta](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="252e2-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="252e2-107">Jälkeen voit luoda tai päivittää DNS palvelua toimialueen (yleensä toimialueen registrar), että DKIM DNS-tietueet, odottaa välitystä DNS-tietueet.</span><span class="sxs-lookup"><span data-stu-id="252e2-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="252e2-108">Jos ei voi luoda DKIM-DNS tietueita admin Centerissä, voit korvata \<CustomDomain\> kanssa mukautetun toimialueen (esimerkiksi contoso.com) ja suorita tämä komento [Exchange Online-PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span><span class="sxs-lookup"><span data-stu-id="252e2-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
