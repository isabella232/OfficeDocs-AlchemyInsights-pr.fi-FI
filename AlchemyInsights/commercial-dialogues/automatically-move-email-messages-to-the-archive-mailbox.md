---
title: Sähköpostiviestien siirtäminen arkistopostilaatikkoon automaattisesti
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746040"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="0671f-102">Sähköpostiviestien siirtäminen arkistopostilaatikkoon automaattisesti</span><span class="sxs-lookup"><span data-stu-id="0671f-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="0671f-103">Näin voit määrittää käytännön, joka siirtää käyttäjän vanhat sähköpostiviestit automaattisesti arkistopostilaatikkoon:</span><span class="sxs-lookup"><span data-stu-id="0671f-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="0671f-104">Siirry [**tietoturvatietojen & tietojen**](https://go.microsoft.com/fwlink/p/?linkid=2077143)hallinta-arkistoon ja tarkista, että käyttäjälle  >    >   on otettu käyttöön arkistopostilaatikko.</span><span class="sxs-lookup"><span data-stu-id="0671f-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="0671f-105">Jos näin ei ole,  valitse **varoitusruudussa** Ota käyttöön ja sitten Kyllä.</span><span class="sxs-lookup"><span data-stu-id="0671f-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="0671f-106">Siirry [**Exchange-hallintakeskukseen > ja säilytystunnisteiden > hallintakeskuksessa.**](https://go.microsoft.com/fwlink/?linkid=2059104)</span><span class="sxs-lookup"><span data-stu-id="0671f-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="0671f-107">Valitse + -kuvake ja valitse sitten **automaattisesti koskee koko postilaatikkoa.**</span><span class="sxs-lookup"><span data-stu-id="0671f-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="0671f-108">Anna säilytystunnisteeseen nimi ja valitse **Siirrä arkistoon.**</span><span class="sxs-lookup"><span data-stu-id="0671f-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="0671f-109">Anna säilytysjaksolle aika, jonka haluat, kuten 90 päivää.</span><span class="sxs-lookup"><span data-stu-id="0671f-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="0671f-110">Valitse **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="0671f-110">Click **Save**.</span></span>
5. <span data-ttu-id="0671f-111">Luo nyt säilytyskäytäntö: valitse **säilytyskäytännöt** ja lisää uusi käytäntö valitsemalla kuvake.</span><span class="sxs-lookup"><span data-stu-id="0671f-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="0671f-112">Määritä säilytyskäytäntöön nimi, etsi ja lisää juuri luomasi säilytystunniste napsauttamalla ja vierittämällä.</span><span class="sxs-lookup"><span data-stu-id="0671f-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="0671f-113">Valitse **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="0671f-113">Click **Save**.</span></span>
7. <span data-ttu-id="0671f-114">Ota lopuksi säilytyskäytäntö käyttöön käyttäjän postilaatikossa: siirry edelleen Exchange-hallintakeskuksessa vastaanottajien   >  **postilaatikoihin.**</span><span class="sxs-lookup"><span data-stu-id="0671f-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="0671f-115">Valitse kaikki käyttäjät, joissa haluat käyttää käytäntöä, ja valitse sitten **Muokkaa** (kynäkuvake).</span><span class="sxs-lookup"><span data-stu-id="0671f-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="0671f-116">Valitse valintaikkunassa **postilaatikon ominaisuudet.**</span><span class="sxs-lookup"><span data-stu-id="0671f-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="0671f-117">Ota **Säilytyskäytäntö-kohdassa** käyttöön juuri luomasi > **tallentaminen.**</span><span class="sxs-lookup"><span data-stu-id="0671f-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="0671f-118">Ohjeet käytännön käyttöönottamisen käyttöön kaikille käyttäjille ovat ohjeaiheessa [Säilytyskäytännön käyttäminen postilaatikoissa.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)</span><span class="sxs-lookup"><span data-stu-id="0671f-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
