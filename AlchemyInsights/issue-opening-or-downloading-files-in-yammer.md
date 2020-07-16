---
title: Tiedostojen avaamiseen tai lataamiseen liittyvä ongelma Yammerissa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148250"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="f0b5e-102">Tiedostojen avaamiseen tai lataamiseen liittyvä ongelma Yammerissa</span><span class="sxs-lookup"><span data-stu-id="f0b5e-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="f0b5e-103">Classic Yammer tukee useita vaihtoehtoja tiedostojen lataamiseen viesteihin ja ryhmiin.</span><span class="sxs-lookup"><span data-stu-id="f0b5e-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="f0b5e-104">Verkon kokoonpanosta riippuen tiedostot ovat oletusarvoisesti tallennustilaa SharePointissa.</span><span class="sxs-lookup"><span data-stu-id="f0b5e-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="f0b5e-105">Uuden Yammerin tiedostovalitsin ei vielä tue kaikkia perinteisessä Yammerissa käytettävissä olevia vaihtoehtoja.</span><span class="sxs-lookup"><span data-stu-id="f0b5e-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="f0b5e-106">Tuleva päivitys lisää lisäominaisuuksia.</span><span class="sxs-lookup"><span data-stu-id="f0b5e-106">A future update will add additional features.</span></span> <span data-ttu-id="f0b5e-107">Lisätietoja on [ohjeaiheessa Tiedoston tai kuvan liittäminen Yammer-keskusteluviestiin](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="f0b5e-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="f0b5e-108">**Tiedoston avaaminen tai lataaminen ei onnistu**</span><span class="sxs-lookup"><span data-stu-id="f0b5e-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="f0b5e-109">Tiedosto saattaa ladata Yammerin, mutta se voidaan linkittää myös SharePoint Onlinen tiedostoon.</span><span class="sxs-lookup"><span data-stu-id="f0b5e-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="f0b5e-110">Vianmääritys edellyttää, että määrität ensin tiedoston sijainnin.</span><span class="sxs-lookup"><span data-stu-id="f0b5e-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="f0b5e-111">Jos tiedosto on ladattu Yammeriin, sillä on \*.yammer.com URL-osoite.</span><span class="sxs-lookup"><span data-stu-id="f0b5e-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="f0b5e-112">Varmista, että tarvittavat URL-osoitteet ja IP-osoitteet poistetaan.</span><span class="sxs-lookup"><span data-stu-id="f0b5e-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="f0b5e-113">Lisätietoja on blogikirjoituksessa [Yammerin kovakoodatut IP-osoitteet ei suositella](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="f0b5e-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="f0b5e-114">Tarkista, voiko käyttäjä, joka on myös yleinen järjestelmänvalvoja, ladata tiedoston.</span><span class="sxs-lookup"><span data-stu-id="f0b5e-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="f0b5e-115">Jos tiedosto on yksityinen, saatat joutua käyttämään yksityistä sisältötilaa.</span><span class="sxs-lookup"><span data-stu-id="f0b5e-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="f0b5e-116">Lisätietoja on kohdassa [Yksityisen sisällön valvonta Yammerissa](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="f0b5e-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="f0b5e-117">**Yammer-verkkotason vieraat ja tiedostot SharePoint Onlinessa**</span><span class="sxs-lookup"><span data-stu-id="f0b5e-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="f0b5e-118">[Yammerin verkkotason vieraat](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) eivät käytä Azure AD B2B:tä ja ovat Yammer-palvelun sisäisiä, joten he eivät voi käyttää SharePointiin tallennettuja Yammer-tiedostoja.</span><span class="sxs-lookup"><span data-stu-id="f0b5e-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="f0b5e-119">Luo ulkoinen AAD B2B -käyttäjä, joka voi käyttää SharePoint Onlinen tiedostokirjastoja kyseisen käyttäjätiedon avulla.</span><span class="sxs-lookup"><span data-stu-id="f0b5e-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="f0b5e-120">Lisätietoja Yammerin tulevasta Azure AD B2B -vierastuesta on kohdassa [Business-to-business (B2B) Vierastuki Yammer Preview'ssa - Asiakkaan käyttöehdot ja usein kysytyt kysymykset](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="f0b5e-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>