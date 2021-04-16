---
title: Poistetun lomakkeen palauttaminen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2547"
- "9000672"
ms.openlocfilehash: 48018accc23a504c34b5469c198d6f29929d25c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809472"
---
# <a name="restore-a-deleted-form"></a><span data-ttu-id="1c926-102">Poistetun lomakkeen palauttaminen</span><span class="sxs-lookup"><span data-stu-id="1c926-102">Restore a deleted form</span></span>

<span data-ttu-id="1c926-103">Jos poistit lomakkeen Microsoft Formsissa vahingossa, voit palauttaa sen.</span><span class="sxs-lookup"><span data-stu-id="1c926-103">If you deleted a form in Microsoft Forms by accident, you can recover it.</span></span> <span data-ttu-id="1c926-104">Kirjaudu Microsoft Formsiin poistetun lomakkeen omistajana.</span><span class="sxs-lookup"><span data-stu-id="1c926-104">Sign in to Microsoft Forms as the owner of the deleted form.</span></span> <span data-ttu-id="1c926-105">Valitse **roskakori**, valitse palautettava lomake ja valitse **sitten Palauta**.</span><span class="sxs-lookup"><span data-stu-id="1c926-105">Select the **Recycle Bin**, then select the form you want to recover and select **Restore**.</span></span> <span data-ttu-id="1c926-106">Kun tiedosto on palautettu, valitse **Takaisin omat lomakkeet -sivun nuoli.**</span><span class="sxs-lookup"><span data-stu-id="1c926-106">Once restored, select the **Back to my Forms page** arrow.</span></span>

<span data-ttu-id="1c926-107">Vain lomakkeen omistaja voi palauttaa sen.</span><span class="sxs-lookup"><span data-stu-id="1c926-107">Only the owner of the form can recover it.</span></span> <span data-ttu-id="1c926-108">Jos lomakkeen omistajan tili on poistettu käytöstä tai poistettu vuokraajassa, vain yleinen järjestelmänvalvoja voi palauttaa lomakkeen.</span><span class="sxs-lookup"><span data-stu-id="1c926-108">If form owner's account was disabled or removed from the tenant, only the Global Administrator can recover the form.</span></span> <span data-ttu-id="1c926-109">Yleisella järjestelmänvalvojalla on oltava Forms-käyttöoikeus, jotta hän voi suorittaa palauttamisen.</span><span class="sxs-lookup"><span data-stu-id="1c926-109">The Global Administrator must have a Forms license to perform a restore.</span></span> <span data-ttu-id="1c926-110">Vain lomakkeet, jotka on luotu 30 päivän kuluessa siitä, kun käyttäjätili poistetaan käytöstä tai poistetaan vuokraajassa, voidaan palauttaa.</span><span class="sxs-lookup"><span data-stu-id="1c926-110">Only forms created within 30 days of the user account being disabled or removed from the tenant can be restored.</span></span>

<span data-ttu-id="1c926-111">Jos olet vuokraajan yleinen järjestelmänvalvoja ja haluat palauttaa lomakkeen tilistä, joka on poistettu tai poistettu käytöstä, korvaa [sähköpostiosoite] poistetun tai käytöstä poistetun käyttäjän sähköpostiosoitteella seuraavassa URL-osoitteessa: **https://forms.office.com/Pages/delegatepage.aspx?originalowner= [sähköpostiosoite]** Jos sähköpostiosoitteesi on johndoe@contoso.com, URL-osoite olisi: **https://forms.office.com/Pages/delegatepage.aspx?originalowner=johndoe@contoso.com** .</span><span class="sxs-lookup"><span data-stu-id="1c926-111">If you are the Global Administrator of the tenant, and you want to recover a form from an account that was deleted or disabled, replace [email address] with the email address of the deleted or disabled user in the following URL: **https://forms.office.com/Pages/delegatepage.aspx?originalowner=[email address]** For example, if your email address is johndoe@contoso.com, the URL would be: **https://forms.office.com/Pages/delegatepage.aspx?originalowner=johndoe@contoso.com**.</span></span> 

<span data-ttu-id="1c926-112">Kun sinulla on käyttöoikeus käyttäjän poistettuihin lomakkeisiin, valitse lomake, jonka haluat siirtää, ja valitse sitten Lisää **lomaketoimintoja**  >  **Siirrä**.</span><span class="sxs-lookup"><span data-stu-id="1c926-112">Once you have access to the user's deleted forms, select the form you want to move, and then select **More Form Actions** > **Move**.</span></span>

<span data-ttu-id="1c926-113">Jos haluat palauttaa lomakkeen, josta se on poistettu ja käyttäjä on poistettu organisaatiosta, yleinen järjestelmänvalvoja voi palauttaa käyttäjän, vaihtaa käyttäjän salasanan ja käyttää lomaketta kirjautuneena sisään toisena aktiivisena käyttäjänä.</span><span class="sxs-lookup"><span data-stu-id="1c926-113">If you want to recover a form where it was deleted and the user was removed from the organization, a Global Administrator can choose to recover the user, reset the password for that user, and then while logged in as that user, access the form to move it to another active user.</span></span> 