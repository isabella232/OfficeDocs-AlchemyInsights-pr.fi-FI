---
title: S/MIME Outlookissa Webissä
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6915470655b85922f6f97e8ca6fac353224b1ae0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/04/2019
ms.locfileid: "36752857"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="081ab-102">Salaa Sähkö posti viestit Outlookissa</span><span class="sxs-lookup"><span data-stu-id="081ab-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="081ab-103">Office 365-sanoman salaus perustuu Microsoft Azure Rights Management (Azure RMS)-tieto suojaan, joka on osa Azure-tietojen suojausta.</span><span class="sxs-lookup"><span data-stu-id="081ab-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="081ab-104">Jos tilauksesi sisältää Azure Rights Management-tai Azure-tietojen suoja uksen, **sinun ei tarvitse ryhtyä mihinkään toimiin oikeuksien hallinta palvelun ottamiseksi käyttöön tai aktivoimiseksi manuaalisesti** .</span><span class="sxs-lookup"><span data-stu-id="081ab-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="081ab-105">Asiakas palautteen perusteella emme enää voi ottaa käyttöön Exchange Mail Flow-sääntöjä salataksesi automaattisesti lähtevän sähkö postin, joka sisältää tietyntyyppisiä arkaluonteisia tietoja vuokraajassasi oletusarvoisesti.</span><span class="sxs-lookup"><span data-stu-id="081ab-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="081ab-106">Sen sijaan annamme yksityiskohtaisia ohjeita siitä, miten voitte tehdä niin itse.</span><span class="sxs-lookup"><span data-stu-id="081ab-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="081ab-107">Lisä tietoja siitä, miten voit luoda kuljetus säännön arkaluonteisten tietojen salaamiseksi, on [tässä artikkelissa](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="081ab-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="081ab-108">Jos käytät Outlookia verkossa (aiemmin **OWA**): Kun kirjoitat Sähkö posti viestiä, klikkaa **suojaa** OWA-selaimessa.</span><span class="sxs-lookup"><span data-stu-id="081ab-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="081ab-109">Tämä koskee "Älä välitä"-lupaa.</span><span class="sxs-lookup"><span data-stu-id="081ab-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="081ab-110">Valitse **Muuta käyttö oikeutta** ja salaa viesti vain valitsemalla **salaa** .</span><span class="sxs-lookup"><span data-stu-id="081ab-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="081ab-111">Jos käytät **Outlook-asiakasta**: Jos haluat lähettää salatun viestin Outlookista 2013 tai 2016 tai Outlook 2016 for Mac, **Valitse asetukset** > -**käyttö oikeudet**ja valitse haluamasi suojaus vaihtoehto.</span><span class="sxs-lookup"><span data-stu-id="081ab-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="081ab-112">Jos haluat **salata automaattisesti kaikki** tietyille vastaanottajille tai ulkopuolisille kumppani organisaatioille lähetetyt sähkö postit, sinun on luotava sähkö postin siirto sääntö Exchange-hallinta keskuksessa.</span><span class="sxs-lookup"><span data-stu-id="081ab-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="081ab-113">[Tässä tuki artikkelissa](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities)on yksityiskohtaisia ohjeita.</span><span class="sxs-lookup"><span data-stu-id="081ab-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

