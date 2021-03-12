---
title: Lähetä sähköpostiviesti antamalla verkkoviestitunnus
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
- "9000760"
- "7391"
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745523"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="cbbe7-102">Lähetä sähköpostiviesti antamalla verkkoviestitunnus</span><span class="sxs-lookup"><span data-stu-id="cbbe7-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="cbbe7-103">Valitse Uusi **lähetys -pikaikkunassa** Sähköposti **ja** **verkkoviestitunnus.**</span><span class="sxs-lookup"><span data-stu-id="cbbe7-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="cbbe7-104">Etsi sähköpostiviestin viestitunnus Outlookissa seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="cbbe7-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="cbbe7-105">Avaa sähköpostiviesti kaksoisnapsauttamalla sitä.</span><span class="sxs-lookup"><span data-stu-id="cbbe7-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="cbbe7-106">Valitse **Tiedoston**  >  **ominaisuudet.**</span><span class="sxs-lookup"><span data-stu-id="cbbe7-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="cbbe7-107">Avaa Muistio tai tyhjä Word-asiakirja ja kopioi ja liitä **sitten Internet-otsikoiden** ruudusta löyty sisältö avoimeen asiakirjaan näkyvyyden parantamiseksi.</span><span class="sxs-lookup"><span data-stu-id="cbbe7-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="cbbe7-108">Etsi **X-MS-Exchange-Organization-Network-Message-Id -kenttä.**</span><span class="sxs-lookup"><span data-stu-id="cbbe7-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="cbbe7-109">Arvo, joka on **lähetyksen** jälkeen: on tunnuksesi.</span><span class="sxs-lookup"><span data-stu-id="cbbe7-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="cbbe7-110">Jos **Vastaanottajat-kohdassa** kaikki tämän sähköpostiviestin vastaanottajat ovat roskapostikansiossa, valitse **Valitse kaikki.**</span><span class="sxs-lookup"><span data-stu-id="cbbe7-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="cbbe7-111">Jos ei, valitse vain käyttäjä, joka ilmoitti ongelmasta.</span><span class="sxs-lookup"><span data-stu-id="cbbe7-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="cbbe7-112">Jos **valitset Lähetyksen syy**-kohdassa Pitäisi olla **estetty,** määritä, onko viesti estetty roskapostina, tietojen kalasteluna tai haittaohjelmana, ja valitse sitten **Lähetä.**</span><span class="sxs-lookup"><span data-stu-id="cbbe7-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="cbbe7-113">Lisätietoja on ohjeaiheessa Roskapostiksi [epäiltyjen roskapostien, tietojen,](https://go.microsoft.com/fwlink/?linkid=2101479)URL-osoitteiden ja tiedostojen lähettäminen Microsoftille tarkistusta varten.</span><span class="sxs-lookup"><span data-stu-id="cbbe7-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
