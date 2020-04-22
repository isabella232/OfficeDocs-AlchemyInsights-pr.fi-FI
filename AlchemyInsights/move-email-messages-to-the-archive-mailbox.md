---
title: Sähköpostiviestien siirtäminen Arkisto-postilaatikkoon
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713643"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="f994f-102">Sähköpostin siirtäminen arkistopostilaatikkoon</span><span class="sxs-lookup"><span data-stu-id="f994f-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="f994f-103">Varmista, että **Arkisto-postilaatikko** on otettu käyttöön.</span><span class="sxs-lookup"><span data-stu-id="f994f-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="f994f-104">Jos näin ei ole, ota arkistopostilaatikko käyttöön [tämän artikkelin](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) ohjeiden mukaisesti.</span><span class="sxs-lookup"><span data-stu-id="f994f-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="f994f-105">Jos haluat arkistoida viestit automaattisesti arkistopostilaatikkoon, säilytystunniste, jossa on **Siirrä arkistoon** -toiminto, on määritettävä **käytettäväksi automaattisesti koko postilaatikossa (oletus) -tunnisteessa.**</span><span class="sxs-lookup"><span data-stu-id="f994f-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="f994f-106">Luo tunniste seuraavasti: [Arkistoi oletustunniste](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="f994f-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="f994f-107">Lisää seuraavaksi **Arkisto-tunniste** säilytyskäytäntöön.</span><span class="sxs-lookup"><span data-stu-id="f994f-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="f994f-108">Valitse Exchange-hallintakeskuksessa **Säilytyskäytännöt** > lisätä **Siirrä arkistoon -tunniste ->** **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="f994f-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="f994f-109">[Määritä säilytyskäytäntö](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) tietyn käyttäjän postilaatikkoon.</span><span class="sxs-lookup"><span data-stu-id="f994f-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="f994f-110">Samaa käytäntöä sovelletaan sekä **Ensisijainen-** että **Arkisto-postilaatikkoon.**</span><span class="sxs-lookup"><span data-stu-id="f994f-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="f994f-111">Saattaa olla tarpeen pakottaa hallitun kansion avustaja (MFA) suorittamaan ja ottamaan uudet asetukset käyttöön käyttäjän postilaatikossa.</span><span class="sxs-lookup"><span data-stu-id="f994f-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="f994f-112">Käynnistä tietyn postilaatikon hallitun kansion hallinta suorittamalla seuraava komento, kun [yhteys on muodostettu EXO PowerShelliin:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="f994f-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="f994f-113">Start-ManagedFolderAssistant -Käyttäjätiedot<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="f994f-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="f994f-114">Lisätietoja arkistokäytännön määrittämisestä on [ohjeaiheessa Postilaatikoiden arkisto- ja poistokäytännön määrittäminen](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="f994f-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  