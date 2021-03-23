---
title: Tuominen ja vieminen Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035437"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="e886a-102">Tuominen ja vieminen Yammer</span><span class="sxs-lookup"><span data-stu-id="e886a-102">Import and export from Yammer</span></span>

<span data-ttu-id="e886a-103">**Tuo**</span><span class="sxs-lookup"><span data-stu-id="e886a-103">**Import**</span></span>

<span data-ttu-id="e886a-104">Käyttäjän tuontiasetukset vaihtelevat sen mukaan, onko Yammer [Microsoft 365:n](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)alkuperäinen tila vai ei.</span><span class="sxs-lookup"><span data-stu-id="e886a-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="e886a-105">**Muu kuin** alkuperäinen tila: Käyttäjät voidaan tuoda ryhmiin käyttämällä Lisää osoitteistosta [-painiketta](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (100 [](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) käyttäjää) ryhmäasetuksissa tai verkostoon käyttämällä verkon järjestelmänvalvojan joukkopäivitystoimintoa.</span><span class="sxs-lookup"><span data-stu-id="e886a-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="e886a-106">**Alkuperäinen tila:** Ryhmän jäsenyys- ja verkoston jäsenyystoiminnot on suoritettava [Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users)-hallintaportaalissa, [Azure AD -portaalissa](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)tai käyttämällä toista Azure AD -vaihtoehtoa.</span><span class="sxs-lookup"><span data-stu-id="e886a-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="e886a-107">Alkuperäistilassa olevat verkostot eivät enää voi käyttää joukkopäivitystä ja muita vanhoja ominaisuuksia.</span><span class="sxs-lookup"><span data-stu-id="e886a-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="e886a-108">Yammer ole koskaan tuettu sisällön tuomista verkoston järjestelmänvalvojalta, vaikka tietojen vientitoimintoa olisi käytetty toisessa verkossa.</span><span class="sxs-lookup"><span data-stu-id="e886a-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="e886a-109">Kumppaniratkaisut tai REST-ohjelmointirajapinnat voivat Yammer uudelleen.</span><span class="sxs-lookup"><span data-stu-id="e886a-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="e886a-110">**Vie**</span><span class="sxs-lookup"><span data-stu-id="e886a-110">**Export**</span></span>

<span data-ttu-id="e886a-111">[Verkoston järjestelmänvalvojan verkostotietojen vieminen](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) sallii sisällön viennin Yammer viesteistä ja tiedostoista.</span><span class="sxs-lookup"><span data-stu-id="e886a-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="e886a-112">Liitteet voivat olla erittäin suuria, ja viennin valmistuminen vie huomattavasti aikaa.</span><span class="sxs-lookup"><span data-stu-id="e886a-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="e886a-113">Suosittelemme, että aktiiviset verkostot viedään [Tietojen vienti -ohjelmointirajapinnan](https://developer.yammer.com/docs/data-export-api) avulla päivittäin tai viikoittain.</span><span class="sxs-lookup"><span data-stu-id="e886a-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="e886a-114">Microsoft-tuki ei tarjoa mukautettuja komentosarjoja tähän tarkoitukseen.</span><span class="sxs-lookup"><span data-stu-id="e886a-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="e886a-115">Yksittäisen käyttäjän [sisällön viemiseen](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) käytetään erillistä GDPR-vientiin.</span><span class="sxs-lookup"><span data-stu-id="e886a-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>