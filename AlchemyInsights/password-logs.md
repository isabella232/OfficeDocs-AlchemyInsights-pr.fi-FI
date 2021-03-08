---
title: Salasanalokit
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/08/2021
ms.locfileid: "50525137"
---
# <a name="password-logs"></a><span data-ttu-id="16c77-102">Salasanalokit</span><span class="sxs-lookup"><span data-stu-id="16c77-102">Password logs</span></span>

<span data-ttu-id="16c77-103">**Minulla on ongelmia salasanan palauttamisen valvontalokien kanssa**</span><span class="sxs-lookup"><span data-stu-id="16c77-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="16c77-104">Suorita seuraava vaihe, jos haluat tehdä vianmääritystä valvontalokien salasanan palauttamiseen liittyvistä ongelmista:</span><span class="sxs-lookup"><span data-stu-id="16c77-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="16c77-105">Varmista, että sinulla on oikeus tarkastella valvontalokeja.</span><span class="sxs-lookup"><span data-stu-id="16c77-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="16c77-106">Vain seuraavat roolit ovat valtuutettuja:</span><span class="sxs-lookup"><span data-stu-id="16c77-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="16c77-107">Yleinen järjestelmänvalvoja</span><span class="sxs-lookup"><span data-stu-id="16c77-107">Global administrator</span></span>
 - <span data-ttu-id="16c77-108">Suojauksen järjestelmänvalvoja</span><span class="sxs-lookup"><span data-stu-id="16c77-108">Security administrator</span></span>
 - <span data-ttu-id="16c77-109">Suojaustietojen lukija</span><span class="sxs-lookup"><span data-stu-id="16c77-109">Security reader</span></span>

<span data-ttu-id="16c77-110">**Haluan nähdä kaikki salasanojen palauttamisen valvontatapahtumat alkuperäisestä käyttöönottoajasta alkaen**</span><span class="sxs-lookup"><span data-stu-id="16c77-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="16c77-111">Jopa 120 000 salasanan vaihto-/rekisteröintitapahtumaa tallennetaan viimeisten 30 päivän raportteihin.</span><span class="sxs-lookup"><span data-stu-id="16c77-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="16c77-112">Tämä enimmäismäärä koskee käyttöliittymää CSV-tiedoston lataamisen yhteydessä.</span><span class="sxs-lookup"><span data-stu-id="16c77-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="16c77-113">Miljoona tapahtumaa on käytettävissä PowerShellin kautta.</span><span class="sxs-lookup"><span data-stu-id="16c77-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="16c77-114">Lisätietoja on alla olevien linkkien kautta:</span><span class="sxs-lookup"><span data-stu-id="16c77-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="16c77-115">Omatoimiset salasanojen palautustapahtumat Azure AD:n Raporttien ja tapahtumien ohjelmointirajapinnasta</span><span class="sxs-lookup"><span data-stu-id="16c77-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="16c77-116">Salasanan palauttamisen rekisteröintitapahtumien lataaminen nopeasti PowerShellin avulla</span><span class="sxs-lookup"><span data-stu-id="16c77-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="16c77-117">**Haluan lisätietoja salasanojen palauttamisen raportointiominaisuuksista**</span><span class="sxs-lookup"><span data-stu-id="16c77-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="16c77-118">Tarkista, kuka on rekisteröinyt tai palauttamassa salasanoja Azure AD:n salasanalla, palauta valvontalokit Azure-portaalissa Käyttäjät **ja ryhmät -kohdassa.**</span><span class="sxs-lookup"><span data-stu-id="16c77-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="16c77-119">Lisätietoja on seuraavissa linkeissä:</span><span class="sxs-lookup"><span data-stu-id="16c77-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="16c77-120">Yleiskatsaus salasanojen vaihtoraportteihin</span><span class="sxs-lookup"><span data-stu-id="16c77-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="16c77-121">Salasanan vaihtoraporttien tarkasteleminen Azure-portaalissa</span><span class="sxs-lookup"><span data-stu-id="16c77-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="16c77-122">Omatoimiset salasanojen palautustapahtumat Azure AD:n Raporttien ja tapahtumien ohjelmointirajapinnasta</span><span class="sxs-lookup"><span data-stu-id="16c77-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="16c77-123">Salasanan palauttamisen rekisteröintitapahtumien lataaminen nopeasti PowerShellin avulla</span><span class="sxs-lookup"><span data-stu-id="16c77-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


