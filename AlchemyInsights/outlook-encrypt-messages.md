---
title: S/MIME Outlookin verkkoversiossa
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 6bbbf8722dacb8b7d5191d57ce1055a48dcb4dd0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511505"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="b3a4c-102">Salaa sähköpostiviestit Outlookissa</span><span class="sxs-lookup"><span data-stu-id="b3a4c-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="b3a4c-103">Microsoft 365 -sanomien salaus perustuu Azure Information Protectioniin kuuluvaan Microsoft Azure Rights Managementiin (Azure RMS).</span><span class="sxs-lookup"><span data-stu-id="b3a4c-103">Microsoft 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="b3a4c-104">Jos tilauksesi sisältää Azure Rights Managementin tai Azure Information Protectionin, sinun ei tarvitse tehdä mitään toimia oikeuksien hallintapalvelun **manuaaliseen käyttöönottoon tai aktivoimiseen.**</span><span class="sxs-lookup"><span data-stu-id="b3a4c-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="b3a4c-105">Asiakaspalautteen perusteella exchange-sähköpostin kulkusäännöt eivät enää anna Exchange-sähköpostin kulusääntöjä salata automaattisesti lähteviä sähköpostiviestejä, jotka sisältävät oletusarvoisesti tietyntyyppisiä arkaluonteisia tietoja vuokraajassasi.</span><span class="sxs-lookup"><span data-stu-id="b3a4c-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="b3a4c-106">Sen sijaan annamme yksityiskohtaisia ohjeita siitä, miten voitte tehdä niin itse.</span><span class="sxs-lookup"><span data-stu-id="b3a4c-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="b3a4c-107">Lisätietoja siirtosäännön luomisesta arkaluonteisten tietojen salaamista varten on [tässä artikkelissa](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="b3a4c-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="b3a4c-108">Jos käytät Outlookin verkkoversiota (aiemmin **OWA):** Kun kirjoitat sähköpostiviestiä, valitse **Suojaa** OWA:ssa.</span><span class="sxs-lookup"><span data-stu-id="b3a4c-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="b3a4c-109">Tämä koskee Älä välitä -oikeutta.</span><span class="sxs-lookup"><span data-stu-id="b3a4c-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="b3a4c-110">Valitse **Muuta käyttöoikeuksia** ja valitse **Salaa,** jos haluat salata vain viestin.</span><span class="sxs-lookup"><span data-stu-id="b3a4c-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="b3a4c-111">Jos käytät **Outlook-asiakasohjelmaa:** Jos haluat lähettää salatun viestin Outlook 2013:sta tai 2016:sta tai Outlook 2016 for Macista, valitse **Asetukset**  >  **Käyttöoikeudet**ja valitse sitten haluamasi suojausvaihtoehto.</span><span class="sxs-lookup"><span data-stu-id="b3a4c-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="b3a4c-112">Jos haluat **salata automaattisesti kaikki** tietyille vastaanottajille tai ulkoisille kumppaniorganisaatioille lähetetyt sähköpostiviestit, sinun on luotava sähköpostin kulkua koskevan siirtosäännön Exchange-hallintakeskuksessa.</span><span class="sxs-lookup"><span data-stu-id="b3a4c-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="b3a4c-113">Yksityiskohtaiset ohjeet ovat [tässä tukiartikkelissa](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="b3a4c-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

