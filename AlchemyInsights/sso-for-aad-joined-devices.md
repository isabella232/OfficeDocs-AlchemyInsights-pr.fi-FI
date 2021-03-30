---
title: Single-Sign Azure Active Directoryyn liitettyjen laitteiden käyttöön
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51404592"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="0a90c-102">Kertakirjaminen Azure Active Directoryyn yhdistetyissä laitteissa</span><span class="sxs-lookup"><span data-stu-id="0a90c-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="0a90c-103">Jos käytössäsi on paikallinen Active Directory (AD) -ympäristö ja haluat liittyä AD-toimialueeseen liitettyihin tietokoneisiin Azure AD:ssä, voit tehdä tämän tekemällä Azure AD -yhdistelmäliitoksen.</span><span class="sxs-lookup"><span data-stu-id="0a90c-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="0a90c-104">[Toimintaohjeita: Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) -yhdistelmäympäristön käyttöönottoon liittyvien vaiheiden avulla voit toteuttaa Azure AD -yhdistelmäliitoksen ympäristössäsi.</span><span class="sxs-lookup"><span data-stu-id="0a90c-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="0a90c-105">Azure AD:ssä liitettyjen laitteiden määrittäminen paikallisille Single-Sign Käytössä Windows Hello for Businessin avulla</span><span class="sxs-lookup"><span data-stu-id="0a90c-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="0a90c-106">**PRT (Primary Refresh Token) -ongelmat** Ensisijainen päivitystunnus (PRT) on Azure AD -todennuksen tärkeä artefakti Windows 10-, Windows Server 2016- ja sitä uudemmassa versiossa, iOS- ja Android-laitteissa.</span><span class="sxs-lookup"><span data-stu-id="0a90c-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="0a90c-107">Se on JSON Web Token (JWT), joka on erityisesti myönnetty Microsoftin ensimmäisen osapuolen tunnuksen välittäjänä, jotta kertakirjautuminen (SSO) voidaan ottaa käyttöön kaikissa näissä laitteissa käytetyissä sovelluksissa.</span><span class="sxs-lookup"><span data-stu-id="0a90c-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="0a90c-108">Mikä on [ensisijainen päivitystunnus?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)-kohdassa annetaan tietoja siitä, miten PRT myönnetään, käytetään ja suojataan Windows 10 -laitteissa.</span><span class="sxs-lookup"><span data-stu-id="0a90c-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="0a90c-109">**WamDefaultSet: KYLLÄ ja AzureADPrt: KYLLÄ** Nämä kentät ilmaisevat, onko käyttäjä onnistunut todentamaan Azure AD:n, kun hän kirjautuu laitteeseen.</span><span class="sxs-lookup"><span data-stu-id="0a90c-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="0a90c-110">Jos arvot ovat **EI,** se voi olla erääntymispäivä:</span><span class="sxs-lookup"><span data-stu-id="0a90c-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="0a90c-111">Laitteeseen liitetyn TPM:n virheellinen tallennustilaavain rekisteröinnin yhteydessä (tarkista KeySignTest, kun käynnissä on järjestelmänvalvojana).</span><span class="sxs-lookup"><span data-stu-id="0a90c-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="0a90c-112">Vaihtoehtoinen kirjautumistunnus</span><span class="sxs-lookup"><span data-stu-id="0a90c-112">Alternate Login ID</span></span>
- <span data-ttu-id="0a90c-113">HTTP-välityspalvelinta ei löydy</span><span class="sxs-lookup"><span data-stu-id="0a90c-113">HTTP Proxy not found</span></span>

<span data-ttu-id="0a90c-114">Laitteiden vianmääritys dsregcmd-komennolla – [SSO-tila](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="0a90c-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
