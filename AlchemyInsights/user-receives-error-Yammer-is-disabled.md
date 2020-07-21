---
title: Käyttäjä saa virheen AADSTS7000112 Yammer on poistettu käytöstä
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198059"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a><span data-ttu-id="05c40-102">Käyttäjä saa virheen AADSTS7000112 Yammer on poistettu käytöstä</span><span class="sxs-lookup"><span data-stu-id="05c40-102">User receives error AADSTS7000112 Yammer is disabled</span></span>

<span data-ttu-id="05c40-103">Jos näyttöön tulee virhe "AADSTS7000112: Application '00000005-0000-0ff1-ce00-00000000000'(Yammer) on poistettu käytöstä", Azure AD:n palvelun pääkohteessa on ongelma.</span><span class="sxs-lookup"><span data-stu-id="05c40-103">If you receive the error "AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled", a problem exists with the service principal within Azure AD.</span></span> <span data-ttu-id="05c40-104">Järjestelmänvalvoja on saattanut poistaa palvelun pääkäyttäjän käytöstä estääkseen Yammerin käytön.</span><span class="sxs-lookup"><span data-stu-id="05c40-104">An administrator might have disabled the service principal to block access to Yammer.</span></span>

<span data-ttu-id="05c40-105">Palvelun pääkohteen poistamista käytöstä ei suositella, ja se voi aiheuttaa lisäongelmia.</span><span class="sxs-lookup"><span data-stu-id="05c40-105">Disabling the service principal is not recommended and can cause additional issues.</span></span> <span data-ttu-id="05c40-106">Lisätietoja tuetusta lähestymistavasta Yammerin käytön estämiseksi on [ohjeaiheessa Yammer-käytön poistaminen käytöstä Microsoft 365 -käyttäjille](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span><span class="sxs-lookup"><span data-stu-id="05c40-106">For more info about the supported approach to block user access to Yammer, see [Turn off Yammer access for Microsoft 365 users](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).</span></span>  

<span data-ttu-id="05c40-107">Voit korjata tämän ongelman Azure-portaalissa ja palauttaa Yammerin käyttöoikeudet seuraavasti:</span><span class="sxs-lookup"><span data-stu-id="05c40-107">To correct this issue in the Azure Portal and restore user access to Yammer:</span></span>

1.  <span data-ttu-id="05c40-108">Avaa Azure Active Directory -sivu ja valitse vasemman siirtymisruudun **Hallinta-kohdassa** **Yrityssovellukset.**</span><span class="sxs-lookup"><span data-stu-id="05c40-108">Open the Azure Active Directory page, and select **Enterprise applications** under **Manage** in the left navigation pane.</span></span>
3.  <span data-ttu-id="05c40-109">Kirjoita hakuruutuun **Office 365 Yammer** ja avaa asetukset valitsemalla sovelluksen nimi.</span><span class="sxs-lookup"><span data-stu-id="05c40-109">Type **Office 365 Yammer** in the search box, and select the application name to open settings.</span></span>
4.  <span data-ttu-id="05c40-110">Valitse vasemman siirtymisruudun **Hallinta-kohdassa** **Ominaisuudet.**</span><span class="sxs-lookup"><span data-stu-id="05c40-110">Select **Properties** under **Manage** in the left navigation pane.</span></span>
5.  <span data-ttu-id="05c40-111">Määritä **käytössä-arvoksi Käytössä, jotta käyttäjät voivat kirjautua sisään?** **Yes** **Save**</span><span class="sxs-lookup"><span data-stu-id="05c40-111">Set the value of **Enabled for users to sign-in?** to **Yes**, and then select **Save**.</span></span>
6.  <span data-ttu-id="05c40-112">Kirjaudu Yammeriin uudelleen.</span><span class="sxs-lookup"><span data-stu-id="05c40-112">Sign in to Yammer again.</span></span> <span data-ttu-id="05c40-113">Sinun on ehkä tyhjennettävä evästeet.</span><span class="sxs-lookup"><span data-stu-id="05c40-113">You might need to clear cookies.</span></span>

<span data-ttu-id="05c40-114">Voit myös määrittää arvon suorittamalla PowerShell-komentoja.</span><span class="sxs-lookup"><span data-stu-id="05c40-114">Alternatively, run PowerShell commands to set the value.</span></span> <span data-ttu-id="05c40-115">Lisätietoja on [ohjeaiheessa "Anteeksi, mutta sisäänkirjautumisessa on ongelmia" -virhe, kun napsautat Office 365:n Yammer-ruutua.](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="05c40-115">For more info, see ["Sorry, but we're having trouble signing you in" error when you click the Yammer tile in Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365).</span></span> 