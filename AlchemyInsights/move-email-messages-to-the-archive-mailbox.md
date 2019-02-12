---
title: Siirtää sähköpostiviestejä postilaatikon arkisto
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a631af20e28a531a40f078e290239a372c38ab74
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/12/2019
ms.locfileid: "29941703"
---
<span data-ttu-id="4c6cb-p101">Ongelmia arkistoon postilaatikon kohteiden arkistoimisen. Varmista, että olet tehnyt seuraavat toimet:</span><span class="sxs-lookup"><span data-stu-id="4c6cb-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="4c6cb-p102">Vahvista, että **Arkistoi postilaatikko** on käytössä. Jos et arkistoi postilaatikko käyttöön [tämän artikkelin](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) ohjeiden avulla.</span><span class="sxs-lookup"><span data-stu-id="4c6cb-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="4c6cb-106">Valitse Exchange-hallintakeskukseen **Pidätys tunnisteet** **Yhteensopivuuden**hallinta, **pidätys tunnisteen** luominen-toiminnolla **siirtää arkisto** sisältää halutun **Pidätys ikä**.</span><span class="sxs-lookup"><span data-stu-id="4c6cb-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="4c6cb-107">-Admin Keskikaiuttimen **Säilytyskäytännöt**, **Säilytyskäytännön** luominen ja **siirtää arkiston** säilytyksen tunnisteen lisääminen politiikan.</span><span class="sxs-lookup"><span data-stu-id="4c6cb-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="4c6cb-p103">[Säilytyskäytännön määrittäminen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) tietyn käyttäjän postilaatikkoon. Samaa käytäntöä sovelletaan sekä **ensisijaisen** että **Arkistoi** postilaatikko.</span><span class="sxs-lookup"><span data-stu-id="4c6cb-p103">[Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="4c6cb-p104">Käyttäjän postilaatikkoon on nyt siirtää kohteita Arkistoi postilaatikko arkisto-käytäntöä. Saatat joutua pakottamaan hallitun kansion avustajan (MFA) ja uusien asetusten käyttäminen käyttäjän postilaatikkoon. Suorittamalla seuraavan komennon käynnistäminen-hallitun kansion avustajan tietyn postilaatikon samalla [yhdistetty EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) :</span><span class="sxs-lookup"><span data-stu-id="4c6cb-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="4c6cb-113">Lisätietoja arkisto-käytännön määrittämisestä on ohjeaiheessa [arkistoinnin ja poistamisen käytännön postilaatikoita varten määritetty](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="4c6cb-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

