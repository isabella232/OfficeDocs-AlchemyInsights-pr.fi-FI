---
title: 'Sähköpostin lähettäminen tai vastaanottaminen Office 365:lle tai Office 365:stä ei onnistu TLS 1.0: n ja TLS 1.1:n käytöstä poistamisen vuoksi'
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745019"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="9dc59-102">Sähköpostin lähettäminen tai vastaanottaminen Office 365:lle tai Office 365:stä ei onnistu TLS 1.0: n ja TLS 1.1:n käytöstä poistamisen vuoksi</span><span class="sxs-lookup"><span data-stu-id="9dc59-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="9dc59-103">Kuten viestikeskuksen mc229914-jälkeinen viesti on vahvistanut, TLS 1.0- ja TLS 1.1 -poisto aloitettiin Exchange Onlinen postinkulkupäätepisteiden käytön.</span><span class="sxs-lookup"><span data-stu-id="9dc59-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="9dc59-104">Pian Office 365 ei enää hyväksy TLS 1.0- ja TLS 1.1 -sähköpostiyhteyksiä ulkoisista lähteistä.</span><span class="sxs-lookup"><span data-stu-id="9dc59-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="9dc59-105">Exchange Online ei myöskään koskaan käytä TLS 1.0: ta tai 1.1 lähtevän sähköpostin lähettämiseen.</span><span class="sxs-lookup"><span data-stu-id="9dc59-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="9dc59-106">Jos kohtaat ongelmia TLS 1.0:n tai 1.1:n käytöstä poistamisen vuoksi, saatat kohdata yhden seuraavista virheistä:</span><span class="sxs-lookup"><span data-stu-id="9dc59-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="9dc59-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span><span class="sxs-lookup"><span data-stu-id="9dc59-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="9dc59-108">Virhe paikallisen palvelimen Jonon katseluohjelmassa, joka lähettää sähköpostia Officer 365:lle– '421 4.4.2 Yhteys katkesi SocketErrorin vuoksi'</span><span class="sxs-lookup"><span data-stu-id="9dc59-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="9dc59-109">Virhe Lähetä [yhdistinprotokolla -lokissa](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) palvelimessa, joka lähettää sähköpostia Office 365:lle– TLS-neuvottelu epäonnistui virheen SocketError kanssa</span><span class="sxs-lookup"><span data-stu-id="9dc59-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="9dc59-110">Virhe yhdistinprotokollan lähetys- tai vastaanottolokissa – '451 5.7.3 StartTLS-komento on ensin annettava'</span><span class="sxs-lookup"><span data-stu-id="9dc59-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="9dc59-111">Jos ilmenee jokin yllä mainituista virheistä, varmista, että sähköpostia lähettävällä tai vastaanottavalla palvelimella on TLS 1.2 käytössä, tarkistamalla seuraavat rekisteriavaimet:</span><span class="sxs-lookup"><span data-stu-id="9dc59-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="9dc59-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Asiakas] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001**</span><span class="sxs-lookup"><span data-stu-id="9dc59-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="9dc59-113">Jos teet muutoksia yllä mainittuihin rekisteriavaimiin TLS 1.2:n käyttöönottoon, käynnistä palvelin uudelleen, jotta muutokset tulevat voimaan.</span><span class="sxs-lookup"><span data-stu-id="9dc59-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="9dc59-114">Varmista myös, että olet asentanut uusimmat Windows- ja Exchange-päivitykset.</span><span class="sxs-lookup"><span data-stu-id="9dc59-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="9dc59-115">Lisätietoja on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="9dc59-115">For more information, see:</span></span>

- [<span data-ttu-id="9dc59-116">Exchange Serverin TLS-ohjeet, osa 1: Valmistautuminen TLS 1.2:ta varten – Microsoft Tech Community -yhteisö</span><span class="sxs-lookup"><span data-stu-id="9dc59-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="9dc59-117">Exchange Serverin TLS-ohjeet, osa 2: TLS 1.2:n ottaminen käyttöön ja asiakkaiden tunnistaminen, jotka eivät käytä sitä - Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="9dc59-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="9dc59-118">Sähköpostiskenaarioiden ymmärtäminen, jos TLS-versioita ei voi hyväksyä Exchange Onlinen avulla – Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="9dc59-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
