---
title: Jakamiskäytännön luominen, jotta käyttäjät voivat jakaa kalenterinsa organisaation ulkopuolisten käyttäjien kanssa
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
- "3800014"
- "898"
ms.openlocfilehash: 016b915a9e8f7e32d5d393bc47347991866647c7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816269"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a><span data-ttu-id="b95cd-102">Jakamiskäytännön luominen, jotta käyttäjät voivat jakaa kalenterinsa organisaation ulkopuolisten käyttäjien kanssa</span><span class="sxs-lookup"><span data-stu-id="b95cd-102">Create a Sharing Policy to allow your users to share their calendar with people outside your organization</span></span>

1. <span data-ttu-id="b95cd-103">Siirry Microsoft 365 -hallintakeskuksessa kohtaan **Järjestelmänvalvoja** > **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="b95cd-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="b95cd-104">Valitse **Organisaatio** > **Jakaminen**.</span><span class="sxs-lookup"><span data-stu-id="b95cd-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="b95cd-105">Valitse luettelonäkymän Yksittäinen **jakaminen -kohdassa** **Uusi** .</span><span class="sxs-lookup"><span data-stu-id="b95cd-105">In the list view, under **Individual Sharing**, click **New** .</span></span>
4. <span data-ttu-id="b95cd-106">Kirjoita **uudessa jakamiskäytäntössä** jakamiskäytännön nimi Käytännön nimi **-ruutuun.**</span><span class="sxs-lookup"><span data-stu-id="b95cd-106">In **new sharing policy**, type a friendly name for the sharing policy in the **Policy name** box.</span></span>
5. <span data-ttu-id="b95cd-107">Määritä **käytännön**  jakamissäännöt valitsemalla Lisää.</span><span class="sxs-lookup"><span data-stu-id="b95cd-107">Click **Add**  to define the sharing rules for the policy.</span></span>
6. <span data-ttu-id="b95cd-108">Valitse **jakamissäännössä** jokin seuraavista asetuksista ja määritä toimialueet, joiden kanssa haluat jakaa:</span><span class="sxs-lookup"><span data-stu-id="b95cd-108">In **sharing rule**, select one of the following options to specify the domains you want to share with:</span></span>
    - <span data-ttu-id="b95cd-109">**Jakaminen kaikkien toimialueiden kanssa**</span><span class="sxs-lookup"><span data-stu-id="b95cd-109">**Sharing with all domains**</span></span>
    - <span data-ttu-id="b95cd-110">**Jakaminen tietyn toimialueen kanssa**</span><span class="sxs-lookup"><span data-stu-id="b95cd-110">**Sharing with a specific domain**</span></span>
8. <span data-ttu-id="b95cd-111">Jos valitset **Jakaminen tietyn toimialueen kanssa**, kirjoita sen toimialueen nimi, jonka kanssa haluat jakaa tiedoston.</span><span class="sxs-lookup"><span data-stu-id="b95cd-111">If you select **Sharing with a specific domain**, type the name of the domain you want to share with.</span></span> <span data-ttu-id="b95cd-112">Jos sinun on annettava tätä jakamiskäytäntöä varten useampi kuin yksi toimialue, tallenna ensimmäisen toimialueen asetukset ja lisää sitten uusia toimialueita muokkaamalla jakamissääntöjä.</span><span class="sxs-lookup"><span data-stu-id="b95cd-112">If you need to enter more than one domain for this sharing policy, save the settings for the first domain, then edit the sharing rules to add more domains.</span></span>
9. <span data-ttu-id="b95cd-113">Jos haluat määrittää jaettavat tiedot, valitse Jaa **kalenterikansio -valintaruutu** ja valitse sitten jokin seuraavista vaihtoehdoista:</span><span class="sxs-lookup"><span data-stu-id="b95cd-113">To specify the information that can be shared, select the **Share your calendar folder** check box, and then select one of the following options:</span></span>
    - <span data-ttu-id="b95cd-114">**Kalenterin tavoitettavuustiedot ja vain aika**</span><span class="sxs-lookup"><span data-stu-id="b95cd-114">**Calendar free/busy information with time only**</span></span>
    - <span data-ttu-id="b95cd-115">**Kalenterin vapaa/varattu-tiedot sekä aika, aihe ja sijainti**</span><span class="sxs-lookup"><span data-stu-id="b95cd-115">**Calendar free/busy information with time, subject, and location**</span></span>
    - <span data-ttu-id="b95cd-116">**Kaikki kalenterin tapaamistiedot, mukaan lukien aika, aihe, sijainti ja otsikko**</span><span class="sxs-lookup"><span data-stu-id="b95cd-116">**All calendar appointment information, including time, subject, location and title**</span></span>
11. <span data-ttu-id="b95cd-117">Määritä **jakamiskäytännön** säännöt valitsemalla Tallenna.</span><span class="sxs-lookup"><span data-stu-id="b95cd-117">Click **save** to set the rules for the sharing policy.</span></span>
12. <span data-ttu-id="b95cd-118">Jos haluat määrittää tämän jakamiskäytännön uudelle oletusarvoinen jakamiskäytäntö kaikille organisaation käyttäjille, valitse Tee tästä käytännön oletusarvoinen **jakamiskäytäntöni** -valintaruutu.</span><span class="sxs-lookup"><span data-stu-id="b95cd-118">If you want to set this sharing policy as the new default sharing policy for all users in your organization, select the **Make this policy my default sharing policy** check box.</span></span>
13. <span data-ttu-id="b95cd-119">Luo **jakamiskäytäntö** valitsemalla Tallenna.</span><span class="sxs-lookup"><span data-stu-id="b95cd-119">Click **save** to create the sharing policy.</span></span>  

<span data-ttu-id="b95cd-120">**Katso lisätietoja tästä aiheesta seuraavista artikkeleista:**</span><span class="sxs-lookup"><span data-stu-id="b95cd-120">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="b95cd-121">Jakamiskäytännön luominen Exchange Onlinessa</span><span class="sxs-lookup"><span data-stu-id="b95cd-121">Create a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [<span data-ttu-id="b95cd-122">Jakamiskäytännön käyttäminen Exchange Onlinen postilaatikoissa</span><span class="sxs-lookup"><span data-stu-id="b95cd-122">Apply a sharing policy to mailboxes in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [<span data-ttu-id="b95cd-123">Jakamiskäytännön muokkaaminen, poistaminen käytöstä tai poistaminen Exchange Onlinessa</span><span class="sxs-lookup"><span data-stu-id="b95cd-123">Modify, disable, or remove a sharing policy in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)