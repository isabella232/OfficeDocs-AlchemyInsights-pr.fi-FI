---
title: Ehdollinen käyttöoikeus estää minua toimialueeseen yhdistetyllä laitteella
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/20/2021
ms.locfileid: "51036704"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a><span data-ttu-id="aa30b-102">Ehdollinen käyttöoikeus estää minua toimialueeseen yhdistetyllä laitteella</span><span class="sxs-lookup"><span data-stu-id="aa30b-102">I’m getting blocked by Conditional Access with domain joined device</span></span>

<span data-ttu-id="aa30b-103">**Erittäin suositellut työkalut**</span><span class="sxs-lookup"><span data-stu-id="aa30b-103">**Highly Recommended Tools**</span></span>

<span data-ttu-id="aa30b-104">[Laitteen rekisteröinnin vianmääritystyökalu](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – työkalu, joka auttaa laitteen yleisimpiä rekisteröintiongelmia vianmäärityksessä.</span><span class="sxs-lookup"><span data-stu-id="aa30b-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - The tool that helps in troubleshooting the most common device registration issues.</span></span>

<span data-ttu-id="aa30b-105">[Test Device Registration Connectivity -komentosarja](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – komentosarja, joka auttaa varmistamaan, että laite voi käyttää järjestelmätilin laitteen rekisteröinnin päätepisteitä.</span><span class="sxs-lookup"><span data-stu-id="aa30b-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - The script that helps ensuring that a device can access Device Registration endpoints under the system account.</span></span>

<span data-ttu-id="aa30b-106">[Azure AD Device Cleanup -komentosarja](https://github.com/mzmaili/AzureADDeviceCleanup) – komentosarja, jonka avulla voit etsiä ja hallita ympäristösi staattisia laitteita.</span><span class="sxs-lookup"><span data-stu-id="aa30b-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - The script that enables you to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="aa30b-107">Seuraavassa on joitakin yleisiä syitä, miksi ehdollinen käyttöoikeus saattaa epäonnistua toimialueeseen yhdistetyssä laitteessa (Azure AD-yhdistelmäympäristössä).</span><span class="sxs-lookup"><span data-stu-id="aa30b-107">Here are some common reasons why conditional access may be failing a device that has joined a domain (Hybrid Azure AD).</span></span>

1. <span data-ttu-id="aa30b-108">**Laitteessa ei ole Azure AD PRT:tä** – Sinun on varmistettava, että laitteessa on Azure AD:n ensisijainen päivitystunnus (PRT).</span><span class="sxs-lookup"><span data-stu-id="aa30b-108">**There’s no Azure AD PRT on the device** - You need to ensure that the device has Azure AD Primary Refresh Token (PRT).</span></span> <span data-ttu-id="aa30b-109">Lisätietoja PRT:stä on tässä [asiakirjassa.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)</span><span class="sxs-lookup"><span data-stu-id="aa30b-109">For more information about PRT, see this [document](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="aa30b-110">Voit tarkistaa, onko sinulla Azure AD PRT, suorittaa komennon laitteessa ja tarkistaa, onko `dsregcmd/status` AzureAdPrt yhtä suuri kuin "KYLLÄ".</span><span class="sxs-lookup"><span data-stu-id="aa30b-110">To verify if you have Azure AD PRT, you can run `dsregcmd/status` command on the device and verify if “AzureAdPrt” equals “YES”.</span></span>

<span data-ttu-id="aa30b-111">Jos "AzureAdPrt" on "EI", tarkista seuraavat asiat:</span><span class="sxs-lookup"><span data-stu-id="aa30b-111">If "AzureAdPrt" is "NO", check the following:</span></span>

- <span data-ttu-id="aa30b-112">**Riippumatta siitä,** onko ympäristössä AD FS liitetty, eikä se ole käytettävissä käyttäjien kotiverkoissa: Varmista tässä tapauksessa, että käyttäjänimellä sekoitettavat päätepisteet ovat käytettävissä ekstranetistä.</span><span class="sxs-lookup"><span data-stu-id="aa30b-112">**Whether you have a federated environment with AD FS, and it’s unreachable from your users’ home networks**: In this case, ensure that your "usernamemixed" endpoints are accessible from the extranet.</span></span> <span data-ttu-id="aa30b-113">Jos AD FS on VPN-yhteyden takana, varmista, että käyttäjät yhdistävät VPN-yhteyden ja kirjautuvat laitteeseen uudelleen.</span><span class="sxs-lookup"><span data-stu-id="aa30b-113">If your AD FS is behind a VPN, ensure that the users connect to the VPN and re-login to the device.</span></span> <span data-ttu-id="aa30b-114">Lisätietoja on tässä [asiakirjassa.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)</span><span class="sxs-lookup"><span data-stu-id="aa30b-114">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains).</span></span>

- <span data-ttu-id="aa30b-115">**Onko laitteen TPM** viallinen eikä näin voi todentaa laitetta: Tarkista "tpm.msc", onko TPM:n tila valmis.</span><span class="sxs-lookup"><span data-stu-id="aa30b-115">**Whether the device’s TPM is faulty and thus cannot authenticate the device**: Check "tpm.msc" to see if the state of TPM is "Ready".</span></span> <span data-ttu-id="aa30b-116">Jos ei ole, `dsregcmd/leave` suorita ja anna laitteen liittyä uudelleen Azure AD:lle.</span><span class="sxs-lookup"><span data-stu-id="aa30b-116">If not, run `dsregcmd/leave` and let the device re-join to Azure AD.</span></span> <span data-ttu-id="aa30b-117">Yritä sitten uudelleen.</span><span class="sxs-lookup"><span data-stu-id="aa30b-117">Then, try again.</span></span> <span data-ttu-id="aa30b-118">Lisätietoja on tässä [asiakirjassa.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="aa30b-118">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>

- <span data-ttu-id="aa30b-119">**Käytössäsi on kolmannen osapuolen tunnistetietojen toimittaja,** joka ei tue WS-Trust protokollaa.</span><span class="sxs-lookup"><span data-stu-id="aa30b-119">**You’re using a 3rd party identity provider, which does not support WS-Trust protocol**.</span></span> <span data-ttu-id="aa30b-120">Kuten tiedostoissamme on kuvattu, Azure AD:llä yhdistetyt yhdistelmälaitteet eivät toimi tässä tapauksessa.</span><span class="sxs-lookup"><span data-stu-id="aa30b-120">As described in our docs, hybrid Azure AD-joined devices cannot work in this case.</span></span> <span data-ttu-id="aa30b-121">Pyydä tukea henkilöllisyyden palveluntarjoajaltasi.</span><span class="sxs-lookup"><span data-stu-id="aa30b-121">Please work with your Identity provider for support.</span></span>

2. <span data-ttu-id="aa30b-122">Käyttäjät käyttävät Chrome-selainta, jossa ei ole **Windows 10** -tilejä tai Office-laajennusta Chromessa, ei automaattisesti käytä **PRT:tä AAD-liitettyihin tai yhdistelmäympäristöihin** liitettyihin laitteisiin: Tämä johtaa laitepohjaisten ehdollisten käyttöoikeuskäytäntöjen epäonnistumiseen, ja näyttöön tulee Rekisteröimätön laite -virhesanoma.</span><span class="sxs-lookup"><span data-stu-id="aa30b-122">**Users are using Chrome browser without the Windows 10 Accounts** or **Office extension Chrome does not automatically use the PRT on AAD-joined or hybrid-AAD-joined devices**: This leads to failure of any device-based Conditional Access policies, with “Unregistered device” error message displayed.</span></span> <span data-ttu-id="aa30b-123">Jos haluat käyttää Chrome-selainta oikein, sinun on asennettava "Windows 10 -tilit" tai "Office-laajennus käyttäjien Chrome-selaimeen" SCCM:n tai Intunen kautta.</span><span class="sxs-lookup"><span data-stu-id="aa30b-123">To use Chrome browser correctly, you must install the “Windows 10 Accounts” or "Office extension to the users’ Chrome browser" via SCCM or Intune.</span></span> <span data-ttu-id="aa30b-124">Lisätietoja on tässä [asiakirjassa.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)</span><span class="sxs-lookup"><span data-stu-id="aa30b-124">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

<span data-ttu-id="aa30b-125">Jos laajennusta ei voi painaa etäyhteyden kautta, ilmoita käyttäjille, että he asentavat yhden yllä mainituista laajennuksista manuaalisesti, jotta he voivat käyttää sovelluksia laitepohjaisen ehdollisen käyttöoikeuden takana.</span><span class="sxs-lookup"><span data-stu-id="aa30b-125">If it’s not possible to push the extension remotely, notify users to manually install one of the above extensions to access applications behind device-based Conditional Access.</span></span> <span data-ttu-id="aa30b-126">Lisätietoja on tässä [asiakirjassa.](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)</span><span class="sxs-lookup"><span data-stu-id="aa30b-126">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites).</span></span>

3. <span data-ttu-id="aa30b-127">Laite oli liitetty oikein Azure AD -yhdistelmäympäristössä, mutta se poistettiin vahingossa tai poistettiin käytöstä **Azure AD Connectin** tai Azure-portaalin synkronointimuutosten vuoksi: Jos näin käy, laiteobjektia ei enää tunnisteta täysin yhdistetyksi laitteeksi, vaikka AzureAdJoined- ja PRT-tila näkyy kelvollisena laitteessa.</span><span class="sxs-lookup"><span data-stu-id="aa30b-127">**The device was correctly hybrid Azure AD joined, but it was inadvertently deleted or disabled, either due to sync changes in Azure AD Connect or from the Azure portal**: If this happens, the device object is no longer recognized as a fully joined device even though the "AzureAdJoined" and "PRT" status show up as valid on the device.</span></span>

<span data-ttu-id="aa30b-128">Voit korjata ongelman toimiminen laitteissa, joihin ongelma vaikuttaa, ja `dsregcmd/leave` salli heidän ottaa Azure AD uudelleen käyttöön.</span><span class="sxs-lookup"><span data-stu-id="aa30b-128">To fix this issue, run `dsregcmd/leave` on the affected devices and let them rejoin Azure AD.</span></span> <span data-ttu-id="aa30b-129">Lisätietoja on tässä [asiakirjassa.](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)</span><span class="sxs-lookup"><span data-stu-id="aa30b-129">For more information, see this [document](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).</span></span>

> [!NOTE]
> <span data-ttu-id="aa30b-130">Jos laitteissasi on Windows 10:n 1809-päivitys, jossa on VPN/pilvivälityspalvelin ja ilmenee ongelmia AzureAdPrt-tilassa tai missä tahansa sovelluksessa, jossa on SSO-ongelma (outlook ei muodosta yhteyttä postilaatikkoon, vaikka sinulla oli PRT), varmista, että sinulla on tämä korjaus [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) tai huhtikuun kumulatiivinen päivitys [KB4549949,](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) jotta PRT-virhe ei toimi kyseisissä koneissa.</span><span class="sxs-lookup"><span data-stu-id="aa30b-130">If your devices are on Windows 10, 1809 update, with VPN/Cloud Proxy and see issues with "AzureAdPrt" state or any app with SSO problem (outlook not connecting to mailbox even though you had PRT), ensure you have this patch [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) or April cumulative update [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) to prevent PRT failures on those machines.</span></span>

















