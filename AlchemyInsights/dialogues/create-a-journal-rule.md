---
title: Päivyrisäännön luonti
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004299"
- "7677"
ms.openlocfilehash: b0b95f8b6460418d92314dede2ca8bc1326b033e
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524810"
---
# <a name="create-a-journal-rule"></a><span data-ttu-id="8daec-102">Päivyrisäännön luonti</span><span class="sxs-lookup"><span data-stu-id="8daec-102">Create a journal rule</span></span>

<span data-ttu-id="8daec-103">Toimi seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="8daec-103">Here's how:</span></span>

1. <span data-ttu-id="8daec-104">Siirry [Exchange-hallintakeskuksessa](https://go.microsoft.com/fwlink/p/?linkid=2059104)vaatimustenmukaisuuden **hallinnan** päivyrisäännöihin ja valitse  >  sitten **Lisää (+) -kuvake.**</span><span class="sxs-lookup"><span data-stu-id="8daec-104">In the [Exchange admin center](https://go.microsoft.com/fwlink/p/?linkid=2059104), go to **compliance management** > **journal rules**, and then select the **Add (+)** icon.</span></span>
2. <span data-ttu-id="8daec-105">Anna **uudessa päivyrisäännössä** päivyrisäännölle nimi ja kilpaile sitten seuraavien kenttien kanssa:</span><span class="sxs-lookup"><span data-stu-id="8daec-105">In **new journal rule**, provide a name for the journal rule and then compete the following fields:</span></span>  
    - <span data-ttu-id="8daec-106">**Lähetä päivyriraportit** osoitteeseen: Kirjoita sen päivyripostilaatikon osoite, joka vastaanottaa kaikki päivyriraportit.</span><span class="sxs-lookup"><span data-stu-id="8daec-106">**Send journal reports to**: Enter the address of the journaling mailbox that will receive all the journal reports.</span></span>  
    - <span data-ttu-id="8daec-107">**Jos viesti lähetetään vastaanottajalle tai vastaanotetaan lähettäjältä:** määritä vastaanottaja, jolle sääntö kohdennetaan.</span><span class="sxs-lookup"><span data-stu-id="8daec-107">**If the message is sent to or received from**: Specify the recipient that the rule will target.</span></span> <span data-ttu-id="8daec-108">Voit joko valita tietyn vastaanottajan tai käyttää sääntöä kaikissa viesteissä.</span><span class="sxs-lookup"><span data-stu-id="8daec-108">You can either select a specific recipient or apply the rule to all messages.</span></span>  
    - <span data-ttu-id="8daec-109">**Kirjaa seuraavat viestit päivyriin:** Määritä päivyrisäännön laajuus.</span><span class="sxs-lookup"><span data-stu-id="8daec-109">**Journal the following messages**: Specify the scope of the journal rule.</span></span> <span data-ttu-id="8daec-110">Voit kirjata päivyriin vain sisäiset viestit, vain ulkoiset viestit tai kaikki viestit alkuperästä tai kohteesta riippumatta.</span><span class="sxs-lookup"><span data-stu-id="8daec-110">You can journal only the internal messages, only the external messages, or all messages regardless of origin or destination.</span></span>
3. <span data-ttu-id="8daec-111">Luo **päivyrisääntö** valitsemalla Tallenna.</span><span class="sxs-lookup"><span data-stu-id="8daec-111">Select **Save** to create the journal rule.</span></span>
