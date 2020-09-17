---
title: 1065 poistumisesta, lähtevä IP-osoite rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806792"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="132c4-102">Poistumisesta-lähtevien IP-osoitteiden alueet</span><span class="sxs-lookup"><span data-stu-id="132c4-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="132c4-103">Olemme havainneet, että organisaatioosi liittyy mahdollisesti ongelma, joka (jos sitä ei ole korjattu 26. loka kuuta, 2018) saattaa rikkoa sähkö postin kulkua paikallisiin tai ulkoisiin kohteisiin.</span><span class="sxs-lookup"><span data-stu-id="132c4-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="132c4-104">Kuten aiemmin ilmoitettiin, voit yksinkertaistaa IP-osoite alueen hallintaa yhdistämällä Exchange Online Protection (ESIP)-IP-osoite alueet, joita käytetään sähkö postin lähettämiseen ja vastaanottoon Microsoft 365: n ulkopuolella.</span><span class="sxs-lookup"><span data-stu-id="132c4-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="132c4-105">Analyysimme osoittaa, että vähintään yksi sähkö postin kulku yhdistimiin määritetyistä ulkoisista Sähkö posti lähteistä tai kohteista ei hyväksy yhteyksiä [tässä](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)näytetyn IP-osoite alueen kautta.</span><span class="sxs-lookup"><span data-stu-id="132c4-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="132c4-106">Toimi ennen 26 päivää loka kuuta varmistaaksesi, että nämä lähteet ja kohteet hyväksyvät yhteydet kaikkiin julkaistujen Sähkö posti [OSOITTEIDEN IP-osoitteisiin](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="132c4-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="132c4-107">Lisä tietoja tästä muutoksesta on kohdassa viesti keskuksen viestit [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)tai [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="132c4-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="132c4-108">**Huomautus**: Jos olet käyttänyt IP-tai URL-julkaisua aiemmin HTML:n, XML:n ja RSS-syötteiden kautta pääte piste päivityksissä, sinun on myös siirryttävä uusiin verkko palveluihin tämäntyyppisten päivitysten automatisoimiseksi.</span><span class="sxs-lookup"><span data-stu-id="132c4-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="132c4-109">Lisä tietoja on kohdassa [microsoft 365-pääte piste luokat ja microsoft 365 IP-osoite ja URL-verkko palvelu](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="132c4-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
