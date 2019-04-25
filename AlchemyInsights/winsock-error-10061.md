---
title: 1554 Winsock-virhe 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7651effc43cb0c4bc2fbbe5349bb72303943f493
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419977"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="1800a-102">WINSOCK-virhe 10061</span><span class="sxs-lookup"><span data-stu-id="1800a-102">Winsock error 10061</span></span>

<span data-ttu-id="1800a-103">Tämä virhekoodi tarkoittaa sitä, että Office 365 ei voinut muodostaa TCP socket (yhteys) tavoite isännän kanssa.</span><span class="sxs-lookup"><span data-stu-id="1800a-103">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="1800a-104">Tämän virheen Todennäköisin syy on ongelma palomuurin määrityksissä.</span><span class="sxs-lookup"><span data-stu-id="1800a-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="1800a-105">Voit korjata ongelman, tarkista nämä asetukset:</span><span class="sxs-lookup"><span data-stu-id="1800a-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="1800a-106">Tietoja [Office 365: n URL-osoitteet ja IP-osoitealueita](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) palomuurin asetusten tarkistaminen</span><span class="sxs-lookup"><span data-stu-id="1800a-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="1800a-107">Jos virhe liittyy, Exchange Online Protection (EOP), sinun olisi aiemmin ilmoitettu muutos [Exchange Online Protection IP-osoitteet](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="1800a-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="1800a-108">Varmista, että Internet-palveluntarjoajan (ISP) Estä portti.</span><span class="sxs-lookup"><span data-stu-id="1800a-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="1800a-109">Tarkista smart isäntä- ja palvelimen asetukset yhdistimet.</span><span class="sxs-lookup"><span data-stu-id="1800a-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="1800a-110">Huomaa, että Office 365 ei estä *saapuvat* yhteydet tällä tavalla.</span><span class="sxs-lookup"><span data-stu-id="1800a-110">Note that Office 365 doesn't block *incoming* connections in this manner.</span></span>
