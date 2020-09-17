---
title: Sähkö posti viestien siirtäminen Arkisto posti laatikkoon
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799777"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="3f355-102">Sähkö postin siirtäminen Arkisto posti laatikkoon</span><span class="sxs-lookup"><span data-stu-id="3f355-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="3f355-103">Jos haluat, että suoritat automaattiset tarkistukset alla mainittuihin asetuksiin, valitse Edellinen-painike <--sivun yläosassa ja kirjoita sitten sen käyttäjän Sähkö posti osoite, jolla on ongelmia sähkö postin siirtämiselle Arkisto posti laatikkoon.</span><span class="sxs-lookup"><span data-stu-id="3f355-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="3f355-104">Varmista, että **Arkisto posti laatikko** on otettu käyttöön.</span><span class="sxs-lookup"><span data-stu-id="3f355-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="3f355-105">Jos näin ei ole, ota Arkisto posti laatikko käyttöön [tämän artikkelin](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) ohjeiden mukaisesti.</span><span class="sxs-lookup"><span data-stu-id="3f355-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="3f355-106">Jos haluat arkistoida viestit automaattisesti Arkisto-posti laatikkoon, **Siirrä arkistoon** -toiminnon sisältävä säilytys tunniste on määritettävä niin, että se otetaan **käyttöön automaattisesti koko posti laatikko (oletus)-tunnisteelle**.</span><span class="sxs-lookup"><span data-stu-id="3f355-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="3f355-107">Luo tunniste seuraavasti: [Arkistoi oletus tunniste](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="3f355-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="3f355-108">Lisää sitten **Arkisto** tunniste säilytys käytäntöön.</span><span class="sxs-lookup"><span data-stu-id="3f355-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="3f355-109">Valitse Exchange-hallinta keskuksessa **säilytys käytännöt** > Lisää **Siirrä arkistoon-tunniste** käytäntöön > **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="3f355-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="3f355-110">[Liitä nyt säilytys käytännön](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) tietyn käyttäjän posti laatikkoon.</span><span class="sxs-lookup"><span data-stu-id="3f355-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="3f355-111">Samaa käytäntöä sovelletaan sekä **perus** -että **Arkisto** posti laatikkoon.</span><span class="sxs-lookup"><span data-stu-id="3f355-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="3f355-112">On ehkä tarpeen pakottaa hallitun kansion avustaja (MFA) suorittamaan uudet asetukset käyttäjän posti laatikkoon ja käyttämään niitä.</span><span class="sxs-lookup"><span data-stu-id="3f355-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="3f355-113">Suorita seuraava komento, kun olet [muodostanut yhteyden EXO PowerShelliin](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) tietyn posti laatikon hallittujen kansioiden hallinnan aloittamiseksi:</span><span class="sxs-lookup"><span data-stu-id="3f355-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="3f355-114">Käynnistä-Managedfoldadassistant-Identity <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="3f355-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="3f355-115">Lisä tietoja arkistointi käytäntöjen määrittämisestä on kohdassa [Arkisto-ja poisto käytäntöjen määrittäminen Posti laatikoille](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="3f355-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  