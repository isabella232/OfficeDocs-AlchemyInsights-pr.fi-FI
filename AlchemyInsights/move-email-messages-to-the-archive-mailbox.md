---
title: Sähkö posti viestien siirtäminen arkiston posti laatikkoon
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822159"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="534ec-102">Sähkö postin siirtäminen arkiston posti laatikkoon</span><span class="sxs-lookup"><span data-stu-id="534ec-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="534ec-103">Varmista, että **arkiston posti laatikko** on otettu käyttöön.</span><span class="sxs-lookup"><span data-stu-id="534ec-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="534ec-104">Jos näin ei ole, ota Arkisto-posti laatikko käyttöön [tässä artikkelissa](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) olevien ohjeiden avulla.</span><span class="sxs-lookup"><span data-stu-id="534ec-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="534ec-105">Jos haluat arkistoida viestit automaattisesti Arkisto-posti laatikkoon, säilytys tunniste, jossa on **Siirrä arkistoon** -toiminto, täytyy määrittää **käyttöön automaattisesti koko posti laatikko (oletus)-tunnisteella**.</span><span class="sxs-lookup"><span data-stu-id="534ec-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="534ec-106">Luo tagi: [Arkistoi oletus tunniste](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)tämän ohjeiden avulla.</span><span class="sxs-lookup"><span data-stu-id="534ec-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="534ec-107">Lisää seuraavaksi **Arkisto** tunniste säilytys käytäntöön.</span><span class="sxs-lookup"><span data-stu-id="534ec-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="534ec-108">Valitse Exchangen hallinta keskuksessa **säilytys käytännöt** > Lisää **Siirrä arkistoon-tunnisteeseen** käytäntö > **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="534ec-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="534ec-109">[Määritä nyt säilytys käytäntö](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) tietyn käyttäjän posti laatikkoon.</span><span class="sxs-lookup"><span data-stu-id="534ec-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="534ec-110">Sama käytäntö otetaan käyttöön sekä **ensisijaisessa** että **arkistossa** olevassa posti laatikossa.</span><span class="sxs-lookup"><span data-stu-id="534ec-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="534ec-111">Hallitun kansion apulainen (MFA) voi olla tarpeen pakottaa suorittamaan ja soveltamaan uusia asetuksia käyttäjän posti laatikkoon.</span><span class="sxs-lookup"><span data-stu-id="534ec-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="534ec-112">Suorita seuraava komento ollessaan [yhteydessä EXO PowerShelliin](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) ja Käynnistä hallitun kansion avustaja tietyssä posti laatikossa:</span><span class="sxs-lookup"><span data-stu-id="534ec-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="534ec-113">Start-ManagedFolderAssistant-identiteetti<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="534ec-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="534ec-114">Lisä tietoja arkistointi käytännön määrittämisestä on kohdassa [Posti laatikoiden arkistointi-ja poisto käytännön määrittäminen](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="534ec-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  