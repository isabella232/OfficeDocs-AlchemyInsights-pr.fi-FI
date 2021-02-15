---
title: Käyttäjän allekirjoituksen estäminen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243422"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="db749-102">Käyttäjän allekirjoituksen estäminen</span><span class="sxs-lookup"><span data-stu-id="db749-102">Block user-made email signatures</span></span>

<span data-ttu-id="db749-103">Seuraava ratkaisu koskee vain Outlookin verkkosovelluksessa luotuja sähköpostin allekirjoituksia.</span><span class="sxs-lookup"><span data-stu-id="db749-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="db749-104">Voit estää allekirjoitukset Outlook-sovelluksessa vain, jos käytössäsi on paikallinen Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="db749-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="db749-105">Valitse hallintakeskuksessa **Hallintakeskukset**  >  **Exchange.**</span><span class="sxs-lookup"><span data-stu-id="db749-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="db749-106">Valitse **käyttöoikeudet**  >  **Outlook Web App -käytännöistä.**</span><span class="sxs-lookup"><span data-stu-id="db749-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="db749-107">Valitse käytäntö ja muokkaa sitä napsauttamalla kynäkuvaketta.</span><span class="sxs-lookup"><span data-stu-id="db749-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="db749-108">Valitse **Ominaisuudet Lisää**  >  **asetuksia.**</span><span class="sxs-lookup"><span data-stu-id="db749-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="db749-109">Poista **Käyttäjäkokemus-kohdassa** Sähköpostin **allekirjoitus -valintaruudun** valinta ja valitse **sitten Tallenna.**</span><span class="sxs-lookup"><span data-stu-id="db749-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="db749-110">**Tärkeää:** Jos allekirjoitus on lisätty ennen tämän valintaruudun valinnan poistamista, käyttäjä voi edelleen käyttää sitä.</span><span class="sxs-lookup"><span data-stu-id="db749-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="db749-111">Pyydä häntä poistamaan se.</span><span class="sxs-lookup"><span data-stu-id="db749-111">Ask them to remove it.</span></span>
