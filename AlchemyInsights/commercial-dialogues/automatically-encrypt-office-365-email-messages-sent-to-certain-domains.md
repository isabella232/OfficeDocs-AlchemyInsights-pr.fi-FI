---
title: Tiettyihin toimialueihin lähetettyjen Office 365 -sähköpostiviestien automaattinen salaaminen
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
ms.openlocfilehash: 7fb96a30cd1922bd39a4b99a7ecd869622f3a466
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746053"
---
# <a name="automatically-encrypt-office-365-email-messages-sent-to-certain-domains"></a><span data-ttu-id="4f5aa-102">Tiettyihin toimialueihin lähetettyjen Office 365 -sähköpostiviestien automaattinen salaaminen</span><span class="sxs-lookup"><span data-stu-id="4f5aa-102">Automatically encrypt Office 365 email messages sent to certain domains</span></span>

1. <span data-ttu-id="4f5aa-103">Valitse [Exchange-hallintakeskuksessa](https://outlook.office365.com/ecp/) **postinkulku- > säännöt.**</span><span class="sxs-lookup"><span data-stu-id="4f5aa-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="4f5aa-104">Napsauta Uusi **(+) -kuvaketta** ja valitse sitten Käytä **Office 365 -viestin salausta ja** viestien oikeuksia.</span><span class="sxs-lookup"><span data-stu-id="4f5aa-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="4f5aa-105">Kirjoita **Nimi-kenttään** säännön nimi, kuten Salaa *contoso.com.*</span><span class="sxs-lookup"><span data-stu-id="4f5aa-105">In **Name**, enter a name for the rule, such as *Encrypt messages sent to contoso.com*.</span></span>
4. <span data-ttu-id="4f5aa-106">Valitse **Käytä tätä sääntöä -kohdassa** **Vastaanottaja, > toimialue on**.</span><span class="sxs-lookup"><span data-stu-id="4f5aa-106">In **Apply this rule if**, choose **The recipient > domain is**.</span></span> 
5. <span data-ttu-id="4f5aa-107">Kirjoita toimialueen nimi, kuten **contoso.com.**</span><span class="sxs-lookup"><span data-stu-id="4f5aa-107">Enter the name of the domain, such as **contoso.com**.</span></span>
6. <span data-ttu-id="4f5aa-108">Napsauta Lisää **(+) -kuvaketta** ja valitse **sitten OK.**</span><span class="sxs-lookup"><span data-stu-id="4f5aa-108">Click the **Add (+)** icon, and then click **OK**.</span></span>
7. <span data-ttu-id="4f5aa-109">Valitse Tee **seuraava kenttä -kohdan** vierestä **Valitse yksi.**</span><span class="sxs-lookup"><span data-stu-id="4f5aa-109">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="4f5aa-110">Valitse **rms-mallin** avattavasta valikosta **Salaa** ja valitse sitten **OK.**</span><span class="sxs-lookup"><span data-stu-id="4f5aa-110">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="4f5aa-111">(Jos et näe tätä vaihtoehtoa, se tarkoittaa, että suunnitelmasi ei sisällä automaattista salausta.</span><span class="sxs-lookup"><span data-stu-id="4f5aa-111">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="4f5aa-112">Voit kuitenkin lisätä sen.)</span><span class="sxs-lookup"><span data-stu-id="4f5aa-112">But you can add it!)</span></span>
9. <span data-ttu-id="4f5aa-113">Valitse mikä tahansa valinnainen valinta (luettelosta valinnaisia valintoja, jotka voit tehdä tässä vaiheessa, joista monet voidaan jättää yksinkertaisuuden oletusasetuksella).</span><span class="sxs-lookup"><span data-stu-id="4f5aa-113">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="4f5aa-114">Valitse **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="4f5aa-114">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="4f5aa-115">Voit aina palata takaisin ja muokata tätä sääntöä myöhemmin.</span><span class="sxs-lookup"><span data-stu-id="4f5aa-115">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="4f5aa-116">Lisätietoja salaussääntöjen luomisesta on ohjeaiheessa Postinkulkusääntöjen määrittäminen [sähköpostiviestien salaamiseen Office 365:ssä](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="4f5aa-116">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>