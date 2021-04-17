---
title: Teams-hallintakeskus
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826376"
---
# <a name="teams-admin-center"></a><span data-ttu-id="f22a5-102">Teams-hallintakeskus</span><span class="sxs-lookup"><span data-stu-id="f22a5-102">Teams Admin Center</span></span>

<span data-ttu-id="f22a5-103">Lisätietoja Teamsin hallinnasta [Teams-hallintakeskuksessa](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="f22a5-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="f22a5-104">Jos et voi käyttää Teams-hallintakeskusta, varmista seuraavat asiat:</span><span class="sxs-lookup"><span data-stu-id="f22a5-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="f22a5-105">Vahvista, että olet sallinut oikeat [Office 365:n IP-osoitteet ja URL-osoitteet](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) kaikissa eteisverkon laitteissa (kuten palomuuri) tai paikallisen laitteesi palomuurisäännöissä.</span><span class="sxs-lookup"><span data-stu-id="f22a5-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="f22a5-106">Vahvista, että Teams-hallintaportaalissa käyttämäsi kirjautumistunnus vastaa [Microsoft 365 -hallintakeskuksessa](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) lueteltua käyttäjätunnusta.</span><span class="sxs-lookup"><span data-stu-id="f22a5-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="f22a5-107">Jos käyttäjiä ei näy Teams-hallintakeskuksessa, varmista seuraavat asiat:</span><span class="sxs-lookup"><span data-stu-id="f22a5-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="f22a5-108">Oletko luonut käyttäjiä tai määrittänyt käyttöoikeuksia viimeksi kuluneiden 24 tunnin aikana?</span><span class="sxs-lookup"><span data-stu-id="f22a5-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="f22a5-109">Varmista, että odotat vähintään 24 tuntia ennen tukipyynnön avaamista.</span><span class="sxs-lookup"><span data-stu-id="f22a5-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="f22a5-110">Varmista, että olet määrittänyt oikeat käyttöoikeudet.</span><span class="sxs-lookup"><span data-stu-id="f22a5-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="f22a5-111">Jos käytössäsi on paikallinen Active Directory, varmista, että [paikallisen Active Directoryn ProxyAddresses-kentän msRTCSIP-PrimaryUserAddress-](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) tai SIP-osoite on yksilöllinen ja muoto vastaa muotoa **sip:** Käyttäjän käyttäjänimi [Microsoft 365 -hallintakeskuksesta.](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)</span><span class="sxs-lookup"><span data-stu-id="f22a5-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="f22a5-112">Jos aiot pitää Skype for Business Serverin käyttöönoton ja määrittää käyttäjät kotikäyttöön paikallisesti ja verkossa: seuraa Skype for Business Serverin Ohjauspaneelissa **olevaa "Set up hybrid with Teams and Skype for Business Online"** (Teamsin ja Skype for Business Onlinen yhdistelmäympäristön määrittäminen) -ohjetta ja siirrä käyttäjiä verkossa.</span><span class="sxs-lookup"><span data-stu-id="f22a5-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
