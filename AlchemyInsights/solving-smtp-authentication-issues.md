---
title: SMTP-todennuksen ja vianmäärityksen ottaminen käyttöön
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077648"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="b06af-102">SMTP-todennuksen ja vianmäärityksen ottaminen käyttöön</span><span class="sxs-lookup"><span data-stu-id="b06af-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="b06af-103">Jos haluat ottaa SMTP-todennuksen käyttöön postilaatikossa tai saat "Asiakas ei todennettu"-, "Todennus epäonnistui" tai "SmtpClientAuthentication"-virheen, jossa on koodi 5.7.57 tai 5.7.3 tai 5.7.139, kun yrität välittää sähköpostia todentamalla laitteen tai sovelluksen Microsoft 365:llä, ratkaise ongelma näiden kolmen toiminnon avulla:</span><span class="sxs-lookup"><span data-stu-id="b06af-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="b06af-104">Poista [Azuren suojauksen oletusasetukset käytöstä](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) valitsemalla Ota suojauksen **oletusasetukset käyttöön -asetus** **ei.**</span><span class="sxs-lookup"><span data-stu-id="b06af-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="b06af-105">a.</span><span class="sxs-lookup"><span data-stu-id="b06af-105">a.</span></span> <span data-ttu-id="b06af-106">Kirjaudu Azure-portaaliin suojauksen järjestelmänvalvojana, ehdollisen käyttöoikeuden järjestelmänvalvojana tai yleisenä järjestelmänvalvojana.</span><span class="sxs-lookup"><span data-stu-id="b06af-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="b06af-107">b.</span><span class="sxs-lookup"><span data-stu-id="b06af-107">b.</span></span> <span data-ttu-id="b06af-108">Siirry  **Azure Active Directory >-kansioon.**</span><span class="sxs-lookup"><span data-stu-id="b06af-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="b06af-109">c.</span><span class="sxs-lookup"><span data-stu-id="b06af-109">c.</span></span> <span data-ttu-id="b06af-110">Valitse **Suojauksen oletusasetusten hallinta**.</span><span class="sxs-lookup"><span data-stu-id="b06af-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="b06af-111">d.</span><span class="sxs-lookup"><span data-stu-id="b06af-111">d.</span></span> <span data-ttu-id="b06af-112">Määritä **Ota käyttöön suojauksen oletusasetukset -asetuksena** **Ei.**</span><span class="sxs-lookup"><span data-stu-id="b06af-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="b06af-113">e.</span><span class="sxs-lookup"><span data-stu-id="b06af-113">e.</span></span> <span data-ttu-id="b06af-114">Valitse **Tallenna**.</span><span class="sxs-lookup"><span data-stu-id="b06af-114">Select **Save**.</span></span>

2. <span data-ttu-id="b06af-115">[Ota asiakkaan SMTP-lähetys](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) käyttöön lisensoilussa postilaatikossa.</span><span class="sxs-lookup"><span data-stu-id="b06af-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="b06af-116">a.</span><span class="sxs-lookup"><span data-stu-id="b06af-116">a.</span></span> <span data-ttu-id="b06af-117">Siirry Microsoft 365 -hallintakeskus Aktiiviset **käyttäjät -valikkoon** ja valitse käyttäjä.</span><span class="sxs-lookup"><span data-stu-id="b06af-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="b06af-118">b.</span><span class="sxs-lookup"><span data-stu-id="b06af-118">b.</span></span> <span data-ttu-id="b06af-119">Siirry Sähköposti-välilehteen ja valitse **Sähköpostisovellukset-kohdassa** **Sähköpostisovellusten hallinta**.</span><span class="sxs-lookup"><span data-stu-id="b06af-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="b06af-120">d.</span><span class="sxs-lookup"><span data-stu-id="b06af-120">d.</span></span> <span data-ttu-id="b06af-121">Varmista, **että Todennettu SMTP** on valittuna (käytössä).</span><span class="sxs-lookup"><span data-stu-id="b06af-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="b06af-122">e.</span><span class="sxs-lookup"><span data-stu-id="b06af-122">e.</span></span> <span data-ttu-id="b06af-123">Valitse **Tallenna muutokset**.</span><span class="sxs-lookup"><span data-stu-id="b06af-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="b06af-124">[Poista monimenetelmäinen todentaminen (MFA) käytöstä](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) lisensoilussa postilaatikossa.</span><span class="sxs-lookup"><span data-stu-id="b06af-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="b06af-125">a.</span><span class="sxs-lookup"><span data-stu-id="b06af-125">a.</span></span> <span data-ttu-id="b06af-126">Siirry Microsoft 365 -hallintakeskus ja valitse vasemmassa siirtymisvalikossa **Käyttäjät,**  >  **jotka ovat aktiivisia.**</span><span class="sxs-lookup"><span data-stu-id="b06af-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="b06af-127">b.</span><span class="sxs-lookup"><span data-stu-id="b06af-127">b.</span></span> <span data-ttu-id="b06af-128">Valitse **Monimenetelmäinen todentaminen**.</span><span class="sxs-lookup"><span data-stu-id="b06af-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="b06af-129">c.</span><span class="sxs-lookup"><span data-stu-id="b06af-129">c.</span></span> <span data-ttu-id="b06af-130">Valitse käyttäjä ja poista **Multi-Factor auth käytöstä.**</span><span class="sxs-lookup"><span data-stu-id="b06af-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
