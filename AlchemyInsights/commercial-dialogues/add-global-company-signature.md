---
title: Yleisen yrityksen allekirjoituksen tai vastuuvapauslausekkeen lisääminen kaikille käyttäjille
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
ms.openlocfilehash: ab0d3fc80b41b9017a6917817270438644f770b8
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481822"
---
# <a name="add-a-global-company-signature-or-disclaimer-for-all-users"></a><span data-ttu-id="20e9c-102">Yleisen yrityksen allekirjoituksen tai vastuuvapauslausekkeen lisääminen kaikille käyttäjille</span><span class="sxs-lookup"><span data-stu-id="20e9c-102">Add a global company signature or disclaimer for all users</span></span>

<span data-ttu-id="20e9c-103">Vihje: Koko organisaation kattavaa allekirjoitusta kutsutaan myös vastuuvapauslausekkeeksi riippumatta siitä, mitä se sisältää.</span><span class="sxs-lookup"><span data-stu-id="20e9c-103">Tip: An org-wide signature is also called a disclaimer, regardless of what it includes.</span></span>

1. <span data-ttu-id="20e9c-104">Valitse hallintakeskuksessa **Hallintakeskukset**  >  **Exchange.**</span><span class="sxs-lookup"><span data-stu-id="20e9c-104">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="20e9c-105">Valitse Sähköpostin kulku -kohdassa **Säännöt**.</span><span class="sxs-lookup"><span data-stu-id="20e9c-105">Under Mail flow, choose **Rules**.</span></span>
3. <span data-ttu-id="20e9c-106">Valitse **+** (Lisää) -kuvake ja valitse **Käytä ilmoituksia**.</span><span class="sxs-lookup"><span data-stu-id="20e9c-106">Click the **+** (Add) icon and choose **Apply disclaimers**.</span></span>
4. <span data-ttu-id="20e9c-107">Anna säännölle nimi.</span><span class="sxs-lookup"><span data-stu-id="20e9c-107">Give the rule a name.</span></span>
5. <span data-ttu-id="20e9c-108">Valitse Käytä tätä sääntöä -kohdassa **Käytä kaikissa viesteissä.**</span><span class="sxs-lookup"><span data-stu-id="20e9c-108">Under Apply this rule, choose **Apply to all messages**.</span></span>
6. <span data-ttu-id="20e9c-109">Jätä kohdassa Seuraava **Lisää vastuuvapausilmoitus** valituksi.</span><span class="sxs-lookup"><span data-stu-id="20e9c-109">Under Do the following, leave **Append the disclaimer** selected.</span></span>
7. <span data-ttu-id="20e9c-110">Valitse **Anna teksti** ja kirjoita vastuuvapausilmoitus.</span><span class="sxs-lookup"><span data-stu-id="20e9c-110">Click **Enter text** and type your disclaimer.</span></span>
8. <span data-ttu-id="20e9c-111">Valitse **Valitse yksi,** valitse **Rivitä** varavaihtoehtona ja valitse sitten **OK.**</span><span class="sxs-lookup"><span data-stu-id="20e9c-111">Click **Select one**, choose **Wrap** as a fallback option, and then click **OK**.</span></span> <span data-ttu-id="20e9c-112">Tämä tarkoittaa, että jos vastuuvapauslauseketta ei voi lisätä salauksen tai toisen sähköpostiosoituksen vuoksi, se rivitetään viestikirjekuoreen.</span><span class="sxs-lookup"><span data-stu-id="20e9c-112">This means that if the disclaimer can't be added because of encryption or another mail setting, it will be wrapped in a message envelope.</span></span>
9. <span data-ttu-id="20e9c-113">Jätä **Valvo tätä sääntöä -** vakavuustaso valittuna.</span><span class="sxs-lookup"><span data-stu-id="20e9c-113">Leave **Audit this rule** with severity level selected.</span></span> <span data-ttu-id="20e9c-114">Valitse sitten Matala, Keskitaso tai Korkea viestilokissa käytettäväksi.</span><span class="sxs-lookup"><span data-stu-id="20e9c-114">Then choose Low, Medium, or High to be used in the message log.</span></span>
10. <span data-ttu-id="20e9c-115">Valitsemalla **Pakota** voit ottaa käyttöön vastuuvapauslausekkeen heti, ellet halua ensin kokeilla sitä.</span><span class="sxs-lookup"><span data-stu-id="20e9c-115">Choose **Enforce** to turn on the disclaimer immediately, unless you want to test it first.</span></span>
11. <span data-ttu-id="20e9c-116">Valitsemalla **Lisäasetukset** voit ottaa käyttöön lisäehtoja tai poikkeuksia.</span><span class="sxs-lookup"><span data-stu-id="20e9c-116">Choose **More options** to include additional conditions or exceptions.</span></span>
12. <span data-ttu-id="20e9c-117">Kun olet valmis, valitse **Tallenna.**</span><span class="sxs-lookup"><span data-stu-id="20e9c-117">When finished, click **Save**.</span></span>
13. <span data-ttu-id="20e9c-118">Tarvitsetko lisätietoja?</span><span class="sxs-lookup"><span data-stu-id="20e9c-118">Need more help?</span></span> [<span data-ttu-id="20e9c-119">Katso video vastuuvapausilmoitusten luomisesta tai lue koko artikkeli.</span><span class="sxs-lookup"><span data-stu-id="20e9c-119">Watch a video about creating disclaimers or read the full article.</span></span>](https://support.office.com/article/2d75860f-c527-4352-a7f6-73eba54c0c72?wt.mc_id=Chat_GlobalSignature)