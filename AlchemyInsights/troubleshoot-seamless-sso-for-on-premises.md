---
title: Saumattoman kertakirjautumisen (SSO) vianmääritys paikallisille
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9370"
- "9004357"
ms.openlocfilehash: a8d14b12bfb3b02da0468eee70af26344465a2a2
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816211"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a><span data-ttu-id="38b1b-102">Saumattoman kertakirjautumisen vianmääritys paikallisille</span><span class="sxs-lookup"><span data-stu-id="38b1b-102">Troubleshoot Seamless Single Sign-on (SSO) for on-premises</span></span>

<span data-ttu-id="38b1b-103">Voit ratkaista saumattoman kertakirjautumisen (SSO) ongelmat seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="38b1b-103">To resolve Seamless Single Sign-on (SSO) issues, perform the following steps:</span></span>

<span data-ttu-id="38b1b-104">**Miten azureadsso-tietokoneen tilin Kerberos-salauksen purkuavain otetaan käyttöön?**</span><span class="sxs-lookup"><span data-stu-id="38b1b-104">**How can I roll over the Kerberos decryption key of the AZUREADSSO computer account?**</span></span>

<span data-ttu-id="38b1b-105">On erittäin suositeltavaa, että käytät Kerberos-salauksen purkuavainta vähintään 30 päivän välein.</span><span class="sxs-lookup"><span data-stu-id="38b1b-105">We highly recommend that you roll over the Kerberos decryption key at least every 30 days.</span></span> <span data-ttu-id="38b1b-106">Jos haluat tehdä tämän manuaalisesti, katso ohjeet [Kerberos-salauksen purkunäppäinten käyttöön.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#)</span><span class="sxs-lookup"><span data-stu-id="38b1b-106">To do this manually, see [How to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span></span>

<span data-ttu-id="38b1b-107">**Saumattoman SSO:n määrittäminen**</span><span class="sxs-lookup"><span data-stu-id="38b1b-107">**Configure Seamless SSO**</span></span>

<span data-ttu-id="38b1b-108">Jos haluat ottaa saumattoman kertakirjautumisen käyttöön, noudata [Azure Active Directory Seamless -kertakirjautumisen vaiheita: Pika-aloitustoiminto.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys)</span><span class="sxs-lookup"><span data-stu-id="38b1b-108">To deploy Seamless SSO, follow the steps in [Azure Active Directory Seamless Single Sign-On: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span></span>

<span data-ttu-id="38b1b-109">**Tiedote**</span><span class="sxs-lookup"><span data-stu-id="38b1b-109">**Advisory**</span></span>

- <span data-ttu-id="38b1b-110">[Azure Active Directory Seamless Single Sign-On: Frequently](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) asked questions - In this article, we address frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span><span class="sxs-lookup"><span data-stu-id="38b1b-110">[Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - In this article, we address frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span></span> <span data-ttu-id="38b1b-111">Jatka uuden sisällön tarkistamista.</span><span class="sxs-lookup"><span data-stu-id="38b1b-111">Keep checking back for new content.</span></span>
- <span data-ttu-id="38b1b-112">[Microsoftin&A –](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) Tässä artikkelissa on tietoja siitä, miten voit esittää ominaisuuspyyntöjä tai esittää teknisiä kysymyksiä Seamless SSO:sta.</span><span class="sxs-lookup"><span data-stu-id="38b1b-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - This article provides information on how to make feature requests or ask technical questions about Seamless SSO.</span></span>

<span data-ttu-id="38b1b-113">**Vianmääritys**</span><span class="sxs-lookup"><span data-stu-id="38b1b-113">**Troubleshoot**</span></span>

<span data-ttu-id="38b1b-114">[Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) -kertakirjautumisen vianmääritys – Tämän artikkelin avulla voit etsiä vianmääritystietoja Azure Active Directoryn (Azure AD) Seamless Single Sign-On (Seamless SSO) yleisistä ongelmista.</span><span class="sxs-lookup"><span data-stu-id="38b1b-114">[Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>







