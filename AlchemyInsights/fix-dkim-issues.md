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
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717559"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="4d17e-102">DKIM-asennusongelmien korjaaminen</span><span class="sxs-lookup"><span data-stu-id="4d17e-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="4d17e-103">Jos dkimin käyttöönotossa mukautetussa toimialueella ilmenee ongelmia, toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="4d17e-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="4d17e-104">Useimmat DKIM-asennusongelmat liittyvät virheellisiin DNS-tietueisiin.</span><span class="sxs-lookup"><span data-stu-id="4d17e-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="4d17e-105">Varmista, että DKIM CNAME -tietue **(ei** TXT-tietue) on muotoiltu oikein.</span><span class="sxs-lookup"><span data-stu-id="4d17e-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="4d17e-106">Lisätietoja on tässä [ohjeaiheessa](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="4d17e-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="4d17e-107">Kun olet luonut tai päivittänyt DKIM DNS -tietueet toimialueesi DNS-isännöintipalvelussa (yleensä toimialueen rekisteröintipalvelussa), odota DNS-tietueiden levittämistä.</span><span class="sxs-lookup"><span data-stu-id="4d17e-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="4d17e-108">Jos et voi luoda DKIM DNS -tietueita hallintakeskuksessa, \<voit\> korvata CustomDomain-toimialueen mukautetulla toimialueella (esimerkiksi contoso.com) `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`ja suorittaa tämän komennon Exchange Online [PowerShellissä:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="4d17e-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
