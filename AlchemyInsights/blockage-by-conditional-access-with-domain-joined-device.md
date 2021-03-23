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
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>Ehdollinen käyttöoikeus estää minua toimialueeseen yhdistetyllä laitteella

**Erittäin suositellut työkalut**

[Laitteen rekisteröinnin vianmääritystyökalu](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) – työkalu, joka auttaa laitteen yleisimpiä rekisteröintiongelmia vianmäärityksessä.

[Test Device Registration Connectivity -komentosarja](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) – komentosarja, joka auttaa varmistamaan, että laite voi käyttää järjestelmätilin laitteen rekisteröinnin päätepisteitä.

[Azure AD Device Cleanup -komentosarja](https://github.com/mzmaili/AzureADDeviceCleanup) – komentosarja, jonka avulla voit etsiä ja hallita ympäristösi staattisia laitteita.

Seuraavassa on joitakin yleisiä syitä, miksi ehdollinen käyttöoikeus saattaa epäonnistua toimialueeseen yhdistetyssä laitteessa (Azure AD-yhdistelmäympäristössä).

1. **Laitteessa ei ole Azure AD PRT:tä** – Sinun on varmistettava, että laitteessa on Azure AD:n ensisijainen päivitystunnus (PRT). Lisätietoja PRT:stä on tässä [asiakirjassa.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)

Voit tarkistaa, onko sinulla Azure AD PRT, suorittaa komennon laitteessa ja tarkistaa, onko `dsregcmd/status` AzureAdPrt yhtä suuri kuin "KYLLÄ".

Jos "AzureAdPrt" on "EI", tarkista seuraavat asiat:

- **Riippumatta siitä,** onko ympäristössä AD FS liitetty, eikä se ole käytettävissä käyttäjien kotiverkoissa: Varmista tässä tapauksessa, että käyttäjänimellä sekoitettavat päätepisteet ovat käytettävissä ekstranetistä. Jos AD FS on VPN-yhteyden takana, varmista, että käyttäjät yhdistävät VPN-yhteyden ja kirjautuvat laitteeseen uudelleen. Lisätietoja on tässä [asiakirjassa.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)

- **Onko laitteen TPM** viallinen eikä näin voi todentaa laitetta: Tarkista "tpm.msc", onko TPM:n tila valmis. Jos ei ole, `dsregcmd/leave` suorita ja anna laitteen liittyä uudelleen Azure AD:lle. Yritä sitten uudelleen. Lisätietoja on tässä [asiakirjassa.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)

- **Käytössäsi on kolmannen osapuolen tunnistetietojen toimittaja,** joka ei tue WS-Trust protokollaa. Kuten tiedostoissamme on kuvattu, Azure AD:llä yhdistetyt yhdistelmälaitteet eivät toimi tässä tapauksessa. Pyydä tukea henkilöllisyyden palveluntarjoajaltasi.

2. Käyttäjät käyttävät Chrome-selainta, jossa ei ole **Windows 10** -tilejä tai Office-laajennusta Chromessa, ei automaattisesti käytä **PRT:tä AAD-liitettyihin tai yhdistelmäympäristöihin** liitettyihin laitteisiin: Tämä johtaa laitepohjaisten ehdollisten käyttöoikeuskäytäntöjen epäonnistumiseen, ja näyttöön tulee Rekisteröimätön laite -virhesanoma. Jos haluat käyttää Chrome-selainta oikein, sinun on asennettava "Windows 10 -tilit" tai "Office-laajennus käyttäjien Chrome-selaimeen" SCCM:n tai Intunen kautta. Lisätietoja on tässä [asiakirjassa.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

Jos laajennusta ei voi painaa etäyhteyden kautta, ilmoita käyttäjille, että he asentavat yhden yllä mainituista laajennuksista manuaalisesti, jotta he voivat käyttää sovelluksia laitepohjaisen ehdollisen käyttöoikeuden takana. Lisätietoja on tässä [asiakirjassa.](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)

3. Laite oli liitetty oikein Azure AD -yhdistelmäympäristössä, mutta se poistettiin vahingossa tai poistettiin käytöstä **Azure AD Connectin** tai Azure-portaalin synkronointimuutosten vuoksi: Jos näin käy, laiteobjektia ei enää tunnisteta täysin yhdistetyksi laitteeksi, vaikka AzureAdJoined- ja PRT-tila näkyy kelvollisena laitteessa.

Voit korjata ongelman toimiminen laitteissa, joihin ongelma vaikuttaa, ja `dsregcmd/leave` salli heidän ottaa Azure AD uudelleen käyttöön. Lisätietoja on tässä [asiakirjassa.](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)

> [!NOTE]
> Jos laitteissasi on Windows 10:n 1809-päivitys, jossa on VPN/pilvivälityspalvelin ja ilmenee ongelmia AzureAdPrt-tilassa tai missä tahansa sovelluksessa, jossa on SSO-ongelma (outlook ei muodosta yhteyttä postilaatikkoon, vaikka sinulla oli PRT), varmista, että sinulla on tämä korjaus [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) tai huhtikuun kumulatiivinen päivitys [KB4549949,](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) jotta PRT-virhe ei toimi kyseisissä koneissa.

















