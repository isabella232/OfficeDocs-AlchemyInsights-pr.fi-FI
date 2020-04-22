---
title: 1065 EOP:n lähtevien IP-osoitealueiden POISTOMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704594"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="f18b2-102">EOP:n lähtevien IP-osoitealueiden poisto</span><span class="sxs-lookup"><span data-stu-id="f18b2-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="f18b2-103">Olemme havainneet organisaatiossasi mahdollisen ongelman, joka saattaa (jos sitä ei korjata 26.10.2018 mennessä) saattaa katkaista postivirran paikallisiin tai ulkoisiin kohteisiin.</span><span class="sxs-lookup"><span data-stu-id="f18b2-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="f18b2-104">Kuten aiemmin ilmoitettiin, ip-osoitealueen hallinnan yksinkertaistamiseksi konsolidoimme Exchange Online Protectionin (EOP) IP-osoitealueet, joita käytetään sähköpostin lähettämiseen ja vastaanottamiseen Microsoft 365:n ulkopuolella.</span><span class="sxs-lookup"><span data-stu-id="f18b2-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="f18b2-105">Analyysimme osoittaa, että yksi tai useampi ulkoinen sähköpostilähde tai -kohde, jonka olet määrittänyt postin virtauksen yhdistimissä, ei hyväksy yhteyksiä [tässä](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)näkyviltä IP-osoitealueilta.</span><span class="sxs-lookup"><span data-stu-id="f18b2-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="f18b2-106">Toimi ennen 26.10. [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)</span><span class="sxs-lookup"><span data-stu-id="f18b2-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="f18b2-107">Lisätietoja tästä muutoksesta on ohjeaiheessa Message Centerin viestit [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)tai [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="f18b2-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="f18b2-108">**Huomautus:** Jos käytit aiemmin IP- tai URL-osoitteiden julkaisemista HTML-, XML- ja RSS-muodossa päätepistepäivityksiä varten, sinun on myös siirryttävä uusiin verkkopalveluihin tämäntyyppisten päivitysten automatisoimiseksi.</span><span class="sxs-lookup"><span data-stu-id="f18b2-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="f18b2-109">Lisätietoja on [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)ohjelm.</span><span class="sxs-lookup"><span data-stu-id="f18b2-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
