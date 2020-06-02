---
title: DKIM-asennusongelmien korjaaminen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 8195b0e3fada6da033b2d95b1fc6600e7fa3341e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506771"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="74730-102">DKIM-asennusongelmien korjaaminen</span><span class="sxs-lookup"><span data-stu-id="74730-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="74730-103">Jos sinulla on ongelmia DKIM:n käyttöönotossa mukautetussa toimialueessa, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="74730-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="74730-104">Useimmat DKIM:n asennusongelmat liittyvät virheellisiin DNS-tietueisiin.</span><span class="sxs-lookup"><span data-stu-id="74730-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="74730-105">Varmista, että DKIM CNAME -tietue **(ei** TXT-tietue) on muotoiltu oikein.</span><span class="sxs-lookup"><span data-stu-id="74730-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="74730-106">Lisätietoja on tässä [ohjeaiheessa](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="74730-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="74730-107">Kun olet luonut tai päivittänyt DKIM DNS -tietueet toimialueesi DNS-isännöintipalvelussa (yleensä toimialueen rekisteröintipalvelussa), odota DNS-tietueiden levittämistä.</span><span class="sxs-lookup"><span data-stu-id="74730-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="74730-108">Jos et voi luoda DKIM DNS -tietueita hallintakeskuksessa, voit korvata \<CustomDomain\> sen mukautetulla toimialueella (esimerkiksi contoso.com) ja suorittaa tämän komennon [Exchange Online PowerShellissä](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="74730-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
