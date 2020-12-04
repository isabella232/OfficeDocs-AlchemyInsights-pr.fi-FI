---
title: Microsoft Edgeen sovellettavat kehittyneet todennus konseptit
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573395"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="c4aad-102">Microsoft Edgeen sovellettavat kehittyneet todennus konseptit</span><span class="sxs-lookup"><span data-stu-id="c4aad-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="c4aad-103">Seuraavat ovat Microsoft Edgeen sovellettavat kehittyneet todennus konseptit:</span><span class="sxs-lookup"><span data-stu-id="c4aad-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="c4aad-104">**Ennakoiva todentaminen**</span><span class="sxs-lookup"><span data-stu-id="c4aad-104">**Proactive Authentication**</span></span>

<span data-ttu-id="c4aad-105">Kun otat [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) -käytännöt käyttöön, Microsoft Edge yrittää todentaa kirjautuneet käyttäjät ennakoivasti Microsoft-palveluiden kautta.</span><span class="sxs-lookup"><span data-stu-id="c4aad-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="c4aad-106">Säännöllisin väli ajoin se käyttää online-palvelua tarkistamaan päivitetyn luettelon, joka sisältää ennakoivan todennuksen määrityksen.</span><span class="sxs-lookup"><span data-stu-id="c4aad-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="c4aad-107">Edut: Ennakoiva todentaminen mahdollistaa todennuksen keskeisiin palveluihin, kuten Officen uusi väli lehti-sivulle.</span><span class="sxs-lookup"><span data-stu-id="c4aad-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="c4aad-108">Jos haku kone käyttää Bing-palvelua, ennakoiva todentaminen parantaa osoite rivin suoritus kykyä ja auttaa luomaan yrityksesi tarpeisiin mukautettuja haku tuloksia.</span><span class="sxs-lookup"><span data-stu-id="c4aad-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="c4aad-109">**Windows Hello CredUI NTLM-todennusta varten**</span><span class="sxs-lookup"><span data-stu-id="c4aad-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="c4aad-110">Jos kertakirjautuminen (SSO) ei ole käytettävissä, kun sivusto yrittää kirja utua käyttäjään NTLM-tai neuvottelu mekanismin kautta, tämän ominaisuuden avulla käyttäjä voi jakaa käyttö järjestelmän tunniste tiedot sivuston kanssa ja täyttää todennus haasteen Windows Hello Cred UI-sovelluksen avulla.</span><span class="sxs-lookup"><span data-stu-id="c4aad-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="c4aad-111">Tämä kirjautumisvuo näkyy vain Windows 10: ssä ja vain niille käyttäjille, jotka eivät saa kertakirjautumista NTLM-tai neuvottelu haasteen aikana.</span><span class="sxs-lookup"><span data-stu-id="c4aad-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="c4aad-112">**Automaattisen kirjautumisen käyttäminen tallennettujen Sala sanojen avulla**</span><span class="sxs-lookup"><span data-stu-id="c4aad-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="c4aad-113">Käyttäjät, jotka tallentavat Sala sanat Microsoft Edgessä, voivat ottaa automaattisen kirjautumisen käyttöön sivustoissa, joihin heillä on tallennettuja tunniste tietoja.</span><span class="sxs-lookup"><span data-stu-id="c4aad-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="c4aad-114">Käyttäjät voivat ottaa tämän toiminnon käyttöön tai poistaa sen käytöstä edge://settings/passwords-sovelluksessa, ja voit määrittää sen [Sala sanan hallintaan](https://go.microsoft.com/fwlink/?linkid=2134622) .</span><span class="sxs-lookup"><span data-stu-id="c4aad-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
