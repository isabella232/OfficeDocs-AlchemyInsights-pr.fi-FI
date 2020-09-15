---
title: 1554 WINSOCK-virhe 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698859"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="7323b-102">WINSOCK-virhe 10061</span><span class="sxs-lookup"><span data-stu-id="7323b-102">Winsock error 10061</span></span>

<span data-ttu-id="7323b-103">Tämä virhe koodi tarkoittaa, että Microsoft ei pystynyt muodostamaan TCP-vastaketta (yhteyttä) kohde isäntään.</span><span class="sxs-lookup"><span data-stu-id="7323b-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="7323b-104">Todennäköisin syy tähän virheeseen on palo muurin määrityksessä oleva ongelma.</span><span class="sxs-lookup"><span data-stu-id="7323b-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="7323b-105">Jos haluat korjata ongelman, valitse seuraavat asetukset:</span><span class="sxs-lookup"><span data-stu-id="7323b-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="7323b-106">Palo muurin määritysten tarkistaminen [Microsoft 365-URL-osoitteiden ja IP-osoite alueiden](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges) tiedoilla</span><span class="sxs-lookup"><span data-stu-id="7323b-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="7323b-107">Jos virhe on määritetty Exchange Online Protection (ESIP)-palvelussa, sinun olisi pitänyt olla aiemmin ilmoitettu [Exchange Online Protection-IP-osoitteiden](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)muutokseen.</span><span class="sxs-lookup"><span data-stu-id="7323b-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="7323b-108">Varmista, ettei Internet-palveluntarjoajasi estä porttia.</span><span class="sxs-lookup"><span data-stu-id="7323b-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="7323b-109">Varmista, että yhdistimessä on älykäs isäntä-ja kohde palvelin-asetukset.</span><span class="sxs-lookup"><span data-stu-id="7323b-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="7323b-110">Huomaa, että Microsoft 365 ei estä *saapuvia* yhteyksiä tällä tavalla.</span><span class="sxs-lookup"><span data-stu-id="7323b-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
