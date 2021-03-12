---
title: Esimerkki Microsoft Defender for Office 365:n tietojenkalastelun estokäytännöstä
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
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746852"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="e819c-102">Esimerkki Microsoft Defender for Office 365:n tietojenkalastelun estokäytännöstä</span><span class="sxs-lookup"><span data-stu-id="e819c-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="e819c-103">Nämä asetukset mahdollistavat käytännön nimeltä Toimialue *ja toimitusjohtaja.*</span><span class="sxs-lookup"><span data-stu-id="e819c-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="e819c-104">Tämä käytäntö tarjoaa sekä käyttäjä- että toimialuesuojauksen tekeytymisviestiltä, ja sen jälkeen käytäntöä sovelletaan kaikkiin sähköpostiviesteihin, jotka käyttäjät ovat vastaanottaneet toimialueella.</span><span class="sxs-lookup"><span data-stu-id="e819c-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="e819c-105">Luo ensin käytäntö lisäämällä seuraavat tiedot:</span><span class="sxs-lookup"><span data-stu-id="e819c-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="e819c-106">**Nimi:** Toimialueen ja **toimitusjohtajan kuvaus:** Varmistaa, että toimitusjohtaja ja toimialueesi eivät tekeyty.</span><span class="sxs-lookup"><span data-stu-id="e819c-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="e819c-107">**Käytössä:** Valitse **vastaanottajan toimialue on**.</span><span class="sxs-lookup"><span data-stu-id="e819c-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="e819c-108">Valitse **jokin näistä** ja **valitse** sitten toimialue.</span><span class="sxs-lookup"><span data-stu-id="e819c-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="e819c-109">Valitse **+ Lisää.**</span><span class="sxs-lookup"><span data-stu-id="e819c-109">Select **+ Add**.</span></span> <span data-ttu-id="e819c-110">Valitse luettelossa toimialueen nimen vieressä olevaa valintaruutua (esimerkiksi *contoso.com)* ja valitse **sitten Lisää.**</span><span class="sxs-lookup"><span data-stu-id="e819c-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="e819c-111">Valitse **Valmis.**</span><span class="sxs-lookup"><span data-stu-id="e819c-111">Select **Done**.</span></span>
- <span data-ttu-id="e819c-112">Kun käytäntö on luotu, voit hienosäätää käytäntöä seuraavilla asetuksilla:</span><span class="sxs-lookup"><span data-stu-id="e819c-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="e819c-113">**Käyttäjien lisääminen suojattavaksi:** Lisää tässä esimerkissä vähintään toimitusjohtajan sähköpostiosoite.</span><span class="sxs-lookup"><span data-stu-id="e819c-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="e819c-114">**Suojaa lisäämällä toimialueita:** Lisää organisaatiotoimialue, joka sisältää toimitusjohtajan toimiston.</span><span class="sxs-lookup"><span data-stu-id="e819c-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="e819c-115">**Toimintojen valinta:** **Jos** sähköpostin on lähettänyt tekeytynyt käyttäjä, valitse Ohjaa viesti toiseen sähköpostiosoitteeseen ja kirjoita sitten suojauksenvalvojan sähköpostiosoite (esimerkiksi *securityadmin@contoso.com).* </span><span class="sxs-lookup"><span data-stu-id="e819c-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="e819c-116">Jos **sähköpostin lähettää tekeytynyt toimialue,** valitse **Aseta viesti karanteeniin.**</span><span class="sxs-lookup"><span data-stu-id="e819c-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="e819c-117">**Postilaatikkotiedot:** Tämä asetus on valittuna oletusarvoisesti, kun luot uuden tietojenkalastelukäytännön.</span><span class="sxs-lookup"><span data-stu-id="e819c-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="e819c-118">Jätä tämä asetus **käyttöön,** niin saat parhaan tuloksen.</span><span class="sxs-lookup"><span data-stu-id="e819c-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="e819c-119">**Luotettujen lähettäjien ja toimialueiden lisääminen:** Älä määritä tässä esimerkissä ohitusta.</span><span class="sxs-lookup"><span data-stu-id="e819c-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="e819c-120">Kun olet tarkistanut asetukset, valitse Luo **tämä käytäntö tai** **Tallenna.**</span><span class="sxs-lookup"><span data-stu-id="e819c-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="e819c-121">Lisätietoja on Microsoft [365:n](https://go.microsoft.com/fwlink/?linkid=2092235)tietojenkalastelun torjunnan käytännöt -kohdassa.</span><span class="sxs-lookup"><span data-stu-id="e819c-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
