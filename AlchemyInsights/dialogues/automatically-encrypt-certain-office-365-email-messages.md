---
title: Tiettyjen Office 365 -sähköpostiviestien automaattinen salaaminen
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524897"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="a77f2-102">Tiettyjen Office 365 -sähköpostiviestien automaattinen salaaminen</span><span class="sxs-lookup"><span data-stu-id="a77f2-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="a77f2-103">Voit salata automaattisesti viestit, jotka käyttäjät lähettävät tietyille ulkoisille käyttäjille tai organisaatioille.</span><span class="sxs-lookup"><span data-stu-id="a77f2-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="a77f2-104">Voit tehdä tämän seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="a77f2-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="a77f2-105">Valitse [Exchange-hallintakeskuksessa](https://outlook.office365.com/ecp/) **postinkulku- > säännöt.**</span><span class="sxs-lookup"><span data-stu-id="a77f2-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="a77f2-106">Napsauta Uusi **(+) -kuvaketta** ja valitse sitten Käytä **Office 365 -viestin salausta ja** viestien oikeuksia.</span><span class="sxs-lookup"><span data-stu-id="a77f2-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="a77f2-107">Kirjoita **Nimi-kenttään** säännön nimi, kuten Salaa *DrToniRamos@gmail.com.*</span><span class="sxs-lookup"><span data-stu-id="a77f2-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="a77f2-108">Valitse **Käytä tätä sääntöä -kohdassa** **Vastaanottaja, > on tämä henkilö.**</span><span class="sxs-lookup"><span data-stu-id="a77f2-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="a77f2-109">Valitse **Valitse jäsenet** -ikkunassa sen henkilön nimi, jota haluat salaussäännön koskee, ja valitse sitten **Lisää.**</span><span class="sxs-lookup"><span data-stu-id="a77f2-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="a77f2-110">Kun olet lisännyt käyttäjät, valitse **OK.**</span><span class="sxs-lookup"><span data-stu-id="a77f2-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="a77f2-111">Valitse Tee **seuraava kenttä -kohdan** vierestä **Valitse yksi.**</span><span class="sxs-lookup"><span data-stu-id="a77f2-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="a77f2-112">Valitse **rms-mallin** avattavasta valikosta **Salaa** ja valitse sitten **OK.**</span><span class="sxs-lookup"><span data-stu-id="a77f2-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="a77f2-113">(Jos et näe tätä vaihtoehtoa, se tarkoittaa, että suunnitelmasi ei sisällä automaattista salausta.</span><span class="sxs-lookup"><span data-stu-id="a77f2-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="a77f2-114">Voit kuitenkin lisätä sen.)</span><span class="sxs-lookup"><span data-stu-id="a77f2-114">But you can add it!)</span></span>
9. <span data-ttu-id="a77f2-115">Valitse mikä tahansa valinnainen valinta (luettelosta valinnaisia valintoja, jotka voit tehdä tässä vaiheessa, joista monet voidaan jättää yksinkertaisuuden oletusasetuksella).</span><span class="sxs-lookup"><span data-stu-id="a77f2-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="a77f2-116">Valitse **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="a77f2-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="a77f2-117">Voit aina palata takaisin ja muokata tätä sääntöä myöhemmin.</span><span class="sxs-lookup"><span data-stu-id="a77f2-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="a77f2-118">Lisätietoja salaussääntöjen luomisesta on kohdassa Postinkulkusääntöjen määrittäminen [sähköpostiviestien salaamiseen Office 365:ssä.](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="a77f2-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>

