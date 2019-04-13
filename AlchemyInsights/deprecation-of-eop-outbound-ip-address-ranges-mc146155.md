---
title: 1065 EOP heikentämisestä lähtevien IP osoite rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 17beb1722142d94ea05b67ce5ed1f20f8b11375c
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/13/2019
ms.locfileid: "31858093"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="6f2fd-102">EOP lähtevien IP-osoitealueita heikentämisestä.</span><span class="sxs-lookup"><span data-stu-id="6f2fd-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="6f2fd-103">Havaitsimme mahdollinen ongelma on organisaatio, joka (Jos ei korjata lokakuu 26th, 2018) saattaa katkaista postin kulku tiloissa tai ulkoisiin kohteisiin.</span><span class="sxs-lookup"><span data-stu-id="6f2fd-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="6f2fd-104">Kuin aiemmin toimitettujen IP osoitteen alueen hallinnon yksinkertaistamiseksi olemme kokoamassa Exchange Online Protection (EOP) IP-osoitealueiden, joiden avulla voit lähettää ja vastaanottaa sähköposti-Office 365: n ulkopuolella.</span><span class="sxs-lookup"><span data-stu-id="6f2fd-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365.</span></span> <span data-ttu-id="6f2fd-105">Meidän analyysi osoittaa, että vähintään yksi ulkoisen sähköpostin lähteitä tai kohteita, jonka olet määrittänyt sähköpostin kulkua liittimet eivät ole hyväksyminen yhteydet IP osoite alueita näytetään [Tässä](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="6f2fd-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="6f2fd-106">Toimia ennen kuin lokakuu 26th varmistaakseen, että näitä lähteitä ja kohteita hyväksyy kaikki [julkaistu EOP IP-osoitteet](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)-yhteyksistä.</span><span class="sxs-lookup"><span data-stu-id="6f2fd-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="6f2fd-107">Lisätietoja tästä muutoksesta on Message Center kirjaa, [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)tai [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="6f2fd-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="6f2fd-108">**Huomautus**: Jos olet aiemmin käyttänyt HTML, XML, RSS ja kautta IP- tai URL-Osoitteen julkaiseminen päätepisteen päivitykset, myös syytä siirtää tällaisia päivityksiä automatisoinnin uusi Internet-palveluihin.</span><span class="sxs-lookup"><span data-stu-id="6f2fd-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="6f2fd-109">Lisätietoja [Office 365: ssä päätepisteen luokat ja Office 365: n IP-osoite ja web-palvelun URL-osoite](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="6f2fd-109">For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
