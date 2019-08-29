---
title: S/MIME-Outlook Web
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: f2c047ca31c586c0aa36701e6e7ca9976cfd1734
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/29/2019
ms.locfileid: "36666837"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="f3eca-102">Salaa sähköpostiviestejä Outlookissa</span><span class="sxs-lookup"><span data-stu-id="f3eca-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="f3eca-103">Office 365: n viestin salaus perustuu Microsoftin Azure Rights Management (Azure RMS), joka on osa Azure tietojen suojaaminen.</span><span class="sxs-lookup"><span data-stu-id="f3eca-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="f3eca-104">Jos tilauksesi sisältää Azure Rights Management tai Azure tietojen suojaaminen Rights Management-palvelu **ei tarvitse tehdä mitään toimia manuaalisesti käyttöön otettavat tai Aktivoi** .</span><span class="sxs-lookup"><span data-stu-id="f3eca-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="f3eca-105">Asiakaspalautteen perusteella olemme enää olla otetaan käyttöön salaa automaattisesti lähtevän sähköpostin että vuokralaisen arkaluontoisten tietojen tyypin joka sisältää oletusarvoisesti mail Exchange työnkulkusäännöt.</span><span class="sxs-lookup"><span data-stu-id="f3eca-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="f3eca-106">Olemme sen sijaan tarjoaa yksityiskohtaiset ohjeet, miten voit tehdä sen itsellesi.</span><span class="sxs-lookup"><span data-stu-id="f3eca-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="f3eca-107">Lisätietoja tärkeiden tietojen salaamiseen liikenteen säännön luominen Lue [tämä artikkeli](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="f3eca-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="f3eca-108">Jos käytät Outlook Web (aiemmalta nimeltään **OWA**): luodessasi sähköpostiviestin valitsemalla **Suojaa** Accessissa.</span><span class="sxs-lookup"><span data-stu-id="f3eca-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="f3eca-109">Tämä koskee oikeuksia ”ei välitä tehdä”.</span><span class="sxs-lookup"><span data-stu-id="f3eca-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="f3eca-110">Valitse **Muuta käyttöoikeuksia** ja valitse **Salaa** vain salata viestin.</span><span class="sxs-lookup"><span data-stu-id="f3eca-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="f3eca-111">Jos **Outlook-asiakas**: Jos haluat lähettää salatun viestin 2013 tai 2016 Outlook tai Outlook-2016 Mac, valitse **asetukset** > **käyttöoikeudet**ja valitse suojaus-asetus on.</span><span class="sxs-lookup"><span data-stu-id="f3eca-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="f3eca-112">**Salaa automaattisesti kaikki sähköposti** lähetetään tietyille vastaanottajille tai kumppani ulkoiset organisaatiot joudut luomaan mail transport virtaussäännön Exchange Admin Centerissä.</span><span class="sxs-lookup"><span data-stu-id="f3eca-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="f3eca-113">Yksityiskohtaiset ohjeet [tuen tässä](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities)artikkelissa.</span><span class="sxs-lookup"><span data-stu-id="f3eca-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

