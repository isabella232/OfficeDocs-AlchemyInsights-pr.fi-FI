---
title: N/MIME Outlookin verkko versiossa
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 052149d1f11387246bc1ff24ba48c45b944ba52c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772259"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="1d489-102">Sähkö posti viestien salaaminen Outlookissa</span><span class="sxs-lookup"><span data-stu-id="1d489-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="1d489-103">Microsoft 365-viestin salaus on luotu Microsoft Azure Rights Managementiin (Azure RMS), joka on osa Azure Information Protectionin suojausta.</span><span class="sxs-lookup"><span data-stu-id="1d489-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="1d489-104">Jos tilauksesi sisältää Azure Rights Management-tai Azure Information Protectionin, **sinun ei tarvitse tehdä mitään toimenpiteitä, jotta voit ottaa käyttöön tai aktivoida** oikeuksien hallinta palvelun manuaalisesti.</span><span class="sxs-lookup"><span data-stu-id="1d489-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="1d489-105">Asiakas palautteen perusteella emme enää voi ottaa käyttöön Exchange-sähkö postin kulku sääntöjä, jos haluat automaattisesti salata lähtevän sähkö postin, joka sisältää tietyntyyppiset luottamukselliset tiedot oletusarvoisesti vuokra ajassa.</span><span class="sxs-lookup"><span data-stu-id="1d489-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="1d489-106">Sen sijaan annamme yksityiskohtaisia ohjeita siitä, miten voit tehdä sen itse.</span><span class="sxs-lookup"><span data-stu-id="1d489-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="1d489-107">Lisä tietoja siitä, miten voit luoda luottamukselliset tiedot salaamalla siirto säännön, on [tässä artikkelissa](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="1d489-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="1d489-108">Jos käytät Outlookia verkossa (aiemmin **OWA**): Kun kirjoitat Sähkö posti viestiä, valitse **Protect** in OWA.</span><span class="sxs-lookup"><span data-stu-id="1d489-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="1d489-109">Tämä koskee Älä lähetä edelleen-oikeutta.</span><span class="sxs-lookup"><span data-stu-id="1d489-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="1d489-110">Valitse **Muuta käyttö oikeutta** ja salaa viesti valitsemalla **salaa** .</span><span class="sxs-lookup"><span data-stu-id="1d489-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="1d489-111">Jos käytät **Outlook-asiakas ohjelmaa**: Jos haluat lähettää salatun viestin Outlook 2013 tai 2016 tai Outlook 2016 for Mac, valitse **Asetukset**  >  **Permissions**ja valitse sitten haluamasi suojaus vaihtoehto.</span><span class="sxs-lookup"><span data-stu-id="1d489-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="1d489-112">Jos haluat **salata automaattisesti kaikki** tietyille vastaanottajalle tai ulkoisille kumppaneille lähetetyt sähkö postit, sinun on luotava sähkö postin kulun siirto sääntö Exchange-hallinta keskuksessa.</span><span class="sxs-lookup"><span data-stu-id="1d489-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="1d489-113">Yksityiskohtaiset ohjeet ovat [tässä tuki artikkelissa](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="1d489-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

