---
title: Microsoft Edgen kehittyneen todentamisen käsitteet
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
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398556"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="dbbdd-102">Microsoft Edgen kehittyneen todentamisen käsitteet</span><span class="sxs-lookup"><span data-stu-id="dbbdd-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="dbbdd-103">Seuraavassa ovat Microsoft Edgeen soveltuvat kehittyneen todentamisen käsitteet:</span><span class="sxs-lookup"><span data-stu-id="dbbdd-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="dbbdd-104">**Ennakoiva todennus**</span><span class="sxs-lookup"><span data-stu-id="dbbdd-104">**Proactive Authentication**</span></span>

<span data-ttu-id="dbbdd-105">Kun otat [ProactiveAuthEnabled-käytännön](https://go.microsoft.com/fwlink/?linkid=2134621) käyttöön, Microsoft Edge yrittää todentaa kirjautuneet käyttäjät ennakoivasti Microsoft-palvelujen kautta.</span><span class="sxs-lookup"><span data-stu-id="dbbdd-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="dbbdd-106">Se tarkistaa säännöllisin väliajoin online-palvelun avulla päivitetyn luetteloluettelon, joka sisältää ennakoivaa todennusta koskevat määritykset.</span><span class="sxs-lookup"><span data-stu-id="dbbdd-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="dbbdd-107">Edut: Ennakoiva todentaminen mahdollistaa todennuksen tärkeimpiin palveluihin, kuten Officen Uusi välilehti -sivuun.</span><span class="sxs-lookup"><span data-stu-id="dbbdd-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="dbbdd-108">Jos Bing-palvelua käytetään hakukoneena, ennakoiva todennus parantaa osoitepalkin suorituskykyä ja auttaa luomaan yrityksesi tarpeita mukautettuja hakutuloksia.</span><span class="sxs-lookup"><span data-stu-id="dbbdd-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="dbbdd-109">**Windows Hello CredUI NTLM-todennukseen**</span><span class="sxs-lookup"><span data-stu-id="dbbdd-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="dbbdd-110">Jos kertakirjautuminen (SSO) ei ole käytettävissä, kun sivusto yrittää kirjautua käyttäjääN NTLM- tai Negotiate-mekanismin avulla, käyttäjä voi jakaa käyttöjärjestelmän tunnistetiedot sivuston kanssa ja täyttää todennushaasteen Windows Hello Cred -käyttöliittymän avulla.</span><span class="sxs-lookup"><span data-stu-id="dbbdd-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="dbbdd-111">Tämä kirjautumisvirta näkyy vain Windows 10:ssä ja vain käyttäjille, jotka eivät saa SSO-kirjautumista NTLM- tai Negotiate-haasteen aikana.</span><span class="sxs-lookup"><span data-stu-id="dbbdd-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="dbbdd-112">**Automaattinen kirjautuminen tallennettujen salasanojen avulla**</span><span class="sxs-lookup"><span data-stu-id="dbbdd-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="dbbdd-113">Käyttäjät, jotka tallentavat salasanoja Microsoft Edgeen, voivat ottaa käyttöön automaattisen kirjautumisen sivustoihin, joissa he ovat tallentaneet tunnistetietoja.</span><span class="sxs-lookup"><span data-stu-id="dbbdd-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="dbbdd-114">Käyttäjät voivat ottaa tämän ominaisuuden käyttöön tai poistaa sen edge://settings/passwords, ja voit määrittää sen salasanojen hallinnan [käytännöistä.](https://go.microsoft.com/fwlink/?linkid=2134622)</span><span class="sxs-lookup"><span data-stu-id="dbbdd-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
