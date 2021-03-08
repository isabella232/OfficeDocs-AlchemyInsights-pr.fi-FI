---
title: Tiettyjen sähköpostiviestien automaattinen salaaminen Office 365:stä
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524909"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="ce1d5-102">Tiettyjen sähköpostiviestien automaattinen salaaminen Office 365:stä</span><span class="sxs-lookup"><span data-stu-id="ce1d5-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="ce1d5-103">Valitse [Exchange-hallintakeskuksessa](https://outlook.office365.com/ecp/) **postinkulku- > säännöt.**</span><span class="sxs-lookup"><span data-stu-id="ce1d5-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="ce1d5-104">Napsauta Uusi **(+) -kuvaketta** ja valitse sitten Käytä **Office 365 -viestin salausta ja** viestien oikeuksia.</span><span class="sxs-lookup"><span data-stu-id="ce1d5-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="ce1d5-105">Kirjoita **Nimi-kenttään** säännön nimi, kuten *Salaa kaikki viestit.*</span><span class="sxs-lookup"><span data-stu-id="ce1d5-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="ce1d5-106">Valitse **Käytä tätä sääntöä jos**-kohdassa **[Käytä kaikissa viesteissä]**.</span><span class="sxs-lookup"><span data-stu-id="ce1d5-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="ce1d5-107">Valitse Tee **seuraava kenttä -kohdan** vierestä **Valitse yksi.**</span><span class="sxs-lookup"><span data-stu-id="ce1d5-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="ce1d5-108">Valitse **rms-mallin** avattavasta valikosta **Salaa** ja valitse sitten **OK.**</span><span class="sxs-lookup"><span data-stu-id="ce1d5-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="ce1d5-109">(Jos et näe tätä vaihtoehtoa, se tarkoittaa, että suunnitelmasi ei sisällä automaattista salausta.</span><span class="sxs-lookup"><span data-stu-id="ce1d5-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="ce1d5-110">Voit kuitenkin lisätä sen.)</span><span class="sxs-lookup"><span data-stu-id="ce1d5-110">But you can add it!)</span></span>
7. <span data-ttu-id="ce1d5-111">Valitse Valvo **tätä sääntöä vakavuustasolla** -valintaruutu ja valitse sitten haluamasi taso.</span><span class="sxs-lookup"><span data-stu-id="ce1d5-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="ce1d5-112">Jos yritykselläsi on sopimusvelvollisuuksia kaikkien salattujen sähköpostiviestien lähettämiseen, suosittelemme, että asetat tasoksi **Korkea.**</span><span class="sxs-lookup"><span data-stu-id="ce1d5-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="ce1d5-113">Valitse **Valitse tämän säännön malli -kohdassa** **Pakota.**</span><span class="sxs-lookup"><span data-stu-id="ce1d5-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="ce1d5-114">Valitse mikä tahansa valinnainen valinta (luettelosta valinnaisia valintoja, jotka voit tehdä tässä vaiheessa, joista monet voidaan jättää yksinkertaisuuden oletusasetuksella).</span><span class="sxs-lookup"><span data-stu-id="ce1d5-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="ce1d5-115">Valitse **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="ce1d5-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="ce1d5-116">Voit aina palata takaisin ja muokata tätä sääntöä myöhemmin.</span><span class="sxs-lookup"><span data-stu-id="ce1d5-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="ce1d5-117">Lisätietoja salaussääntöjen luomisesta on ohjeaiheessa Postinkulkusääntöjen määrittäminen [sähköpostiviestien salaamiseen Office 365:ssä](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="ce1d5-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

