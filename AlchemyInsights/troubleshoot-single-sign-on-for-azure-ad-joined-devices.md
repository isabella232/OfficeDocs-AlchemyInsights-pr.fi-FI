---
title: Kertakirjaaminen Azure AD:ssä liitettyjen laitteiden vianmääritys
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/19/2021
ms.locfileid: "51035468"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="ceaea-102">Kertakirjaaminen Azure AD:ssä liitettyjen laitteiden vianmääritys</span><span class="sxs-lookup"><span data-stu-id="ceaea-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="ceaea-103">Jos sinulla on paikallinen Active Directory (AD) -ympäristö ja haluat liittyä AD-toimialueeseen liitettyihin tietokoneisiin Azure AD:ssä, voit tehdä tämän tekemällä Azure AD -yhdistelmäliitoksen.</span><span class="sxs-lookup"><span data-stu-id="ceaea-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="ceaea-104">[Toimintaohjeita: Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) -yhdistelmäympäristön käyttöönottoon liittyvien vaiheiden avulla voit toteuttaa Azure AD -yhdistelmäliitoksen ympäristössäsi.</span><span class="sxs-lookup"><span data-stu-id="ceaea-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="ceaea-105">Lisätietoja on kohdassa Azure AD:n liitettyjen laitteiden määrittäminen [paikallisille Single-Sign Windows Hello for Businessin käyttöön.](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base)</span><span class="sxs-lookup"><span data-stu-id="ceaea-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="ceaea-106">**PRT (Primary Refresh Token) -ongelmat**</span><span class="sxs-lookup"><span data-stu-id="ceaea-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="ceaea-107">Ensisijainen päivitystunnus (PRT) on Azure AD -todennuksen tärkeä artefakti Windows 10-, Windows Server 2016- ja sitä uudemmassa versiossa, iOS- ja Android-laitteissa.</span><span class="sxs-lookup"><span data-stu-id="ceaea-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="ceaea-108">Se on JSON Web Token (JWT), joka on erityisesti myönnetty Microsoftin ensimmäisen osapuolen tunnuksen välittäjänä, jotta kertakirjautuminen (SSO) voidaan ottaa käyttöön kaikissa näissä laitteissa käytetyissä sovelluksissa.</span><span class="sxs-lookup"><span data-stu-id="ceaea-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="ceaea-109">Lisätietoja PRT:n myöntäjästä, käytössä ja suojasta Windows 10 -laitteissa on ohjeaiheessa Mikä on [ensisijainen päivitystunnus?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="ceaea-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="ceaea-110">**WamDefaultSet: KYLLÄ ja AzureADPrt: KYLLÄ**</span><span class="sxs-lookup"><span data-stu-id="ceaea-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="ceaea-111">Nämä kentät ilmaisevat, onko käyttäjä onnistunut todentamaan Azure AD:n, kun kirjaudut sisään laitteeseen.</span><span class="sxs-lookup"><span data-stu-id="ceaea-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="ceaea-112">Jos arvot ovat **EI,** se voi johtua:</span><span class="sxs-lookup"><span data-stu-id="ceaea-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="ceaea-113">Laitteeseen liitetyn TPM:n virheellinen tallennustilaavain rekisteröinnin yhteydessä (tarkista KeySignTest, kun käynnissä on laajennettuna)</span><span class="sxs-lookup"><span data-stu-id="ceaea-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="ceaea-114">Vaihtoehtoinen kirjautumistunnus</span><span class="sxs-lookup"><span data-stu-id="ceaea-114">Alternate Login ID</span></span>
- <span data-ttu-id="ceaea-115">HTTP-välityspalvelinta ei löydy</span><span class="sxs-lookup"><span data-stu-id="ceaea-115">HTTP Proxy not found</span></span>

<span data-ttu-id="ceaea-116">Lisätietoja laitteiden vianmäärityksestä dsregcmd-komennolla on kohdassa [SSO-tila.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="ceaea-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
