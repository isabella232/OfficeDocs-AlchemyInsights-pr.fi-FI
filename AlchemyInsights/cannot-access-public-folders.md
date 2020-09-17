---
title: Yleisten kansioiden käyttäminen ei onnistu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812544"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="bd894-102">Outlook ei voi muodostaa yhteyttä julkisiin kansioihin</span><span class="sxs-lookup"><span data-stu-id="bd894-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="bd894-103">Jos Julkinen-kansion käyttö ei toimi joillekin käyttäjille, kokeile seuraavaa:</span><span class="sxs-lookup"><span data-stu-id="bd894-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="bd894-104">Muodosta yhteys EXO PowerShelliin ja Määritä ongelman käyttäjä tilillä oleva Defaunpublic-posti laatikko-parametri vastaamaan toimivan käyttäjä tilin parametria.</span><span class="sxs-lookup"><span data-stu-id="bd894-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="bd894-105">Esimerkiksi</span><span class="sxs-lookup"><span data-stu-id="bd894-105">Example:</span></span>

<span data-ttu-id="bd894-106">Get-Mailbox WorkingUser | FT Defaja Publictillbox, Effectivepublikansiposti laatikko</span><span class="sxs-lookup"><span data-stu-id="bd894-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="bd894-107">Posti laatikon ProblemUser-Defauspublicifolder-posti laatikon asettaminen \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="bd894-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="bd894-108">Odota vähintään yksi tunti, ennen kuin muutos tulee voimaan.</span><span class="sxs-lookup"><span data-stu-id="bd894-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="bd894-109">Jos ongelma jatkuu, noudata [näitä ohjeita](https://aka.ms/pfcte) , jotta voit suorittaa yleisten kansioiden käyttö ongelmien vian määrityksen Outlookin avulla.</span><span class="sxs-lookup"><span data-stu-id="bd894-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="bd894-110">Voit **määrittää, ketkä käyttäjät voivat käyttää yleisiä kansioita Outlookin avulla**:</span><span class="sxs-lookup"><span data-stu-id="bd894-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="bd894-111">Käytä joukkoa-CASMailbox <mailboxname> -publickansioasiakaskäyttöoikeus $True tai $false</span><span class="sxs-lookup"><span data-stu-id="bd894-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="bd894-112">$true: Salli käyttäjien käyttää yleisiä kansioita Outlookissa</span><span class="sxs-lookup"><span data-stu-id="bd894-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="bd894-113">$false: Estä Outlookin yleisten kansioiden käyttö.</span><span class="sxs-lookup"><span data-stu-id="bd894-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="bd894-114">Tämä on oletusarvo.</span><span class="sxs-lookup"><span data-stu-id="bd894-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="bd894-115">Asetukset-OrganizationConfig-Publiclickshowclient Control $true</span><span class="sxs-lookup"><span data-stu-id="bd894-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="bd894-116">**Huomautus** Tämä toiminto sarja voi hallita yhteyksiä vain Windows-asiakas ohjelmien Outlookin Työpöytä versiossa.</span><span class="sxs-lookup"><span data-stu-id="bd894-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="bd894-117">Käyttäjä voi edelleen käyttää yleisiä kansioita OWA-tai Outlook for Mac-sovelluksessa.</span><span class="sxs-lookup"><span data-stu-id="bd894-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="bd894-118">Lisä tietoja on kohdassa [valvottavien yhteyksien tuen ilmoittaminen Outlookin julkisissa kansioissa](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="bd894-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>