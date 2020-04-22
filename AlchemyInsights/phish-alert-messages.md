---
title: 2491 Ilmoita Phish Delivered -palvelun sähköpostiviestit vuokralaisen tai käyttäjän ohituskäytännön vuoksi
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758921"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="af180-102">Ilmoita Phish Delivered -palvelun sähköpostiviestit vuokraajan tai käyttäjän ohituksen vuoksi -käytännöstä</span><span class="sxs-lookup"><span data-stu-id="af180-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="af180-103">Oletushälytyskäytäntö nimeltä "Phish Toimitettu vuokraajan tai käyttäjän ohituksen vuoksi" on otettu käyttöön vuokraajille, joilla on Office 365 ATP P1- ja P2-käyttöoikeudet.</span><span class="sxs-lookup"><span data-stu-id="af180-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="af180-104">Jos sait tämän ilmoituksen, voit tutkia seuraavia ohjeita:</span><span class="sxs-lookup"><span data-stu-id="af180-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="af180-105">Siirry Suojaus-& yhteensopivuuskeskuksen **Hälytykset-sivulle** valitsemalla **ilmoitusviestin.**</span><span class="sxs-lookup"><span data-stu-id="af180-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="af180-106">Valitse ilmoitus, jos haluat nähdä vaihtoehdon **Näytä viestiluettelo** tai **Näytä viestit Resurssienhallinnassa**.</span><span class="sxs-lookup"><span data-stu-id="af180-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="af180-107">Molemmat näistä vaihtoehdoista vievät viestin tiedot, jotka sisältävät viestin tunnuksen.</span><span class="sxs-lookup"><span data-stu-id="af180-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="af180-108">Huomaa, että Threat Explorer -linkki suodattaa automaattisesti sanomaehtoja vastaavat viestit.</span><span class="sxs-lookup"><span data-stu-id="af180-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="af180-109">Päivämääräsuodatinta on ehkä muutettava Threat Explorerissa.</span><span class="sxs-lookup"><span data-stu-id="af180-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="af180-110">Tietojenkalasteluviesti toimitettiin manuaalisesti määritetyn ohituksen vuoksi:</span><span class="sxs-lookup"><span data-stu-id="af180-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="af180-111">Käyttäjän määrittämä sallittu lähettäjä tai toimialue.</span><span class="sxs-lookup"><span data-stu-id="af180-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="af180-112">Järjestelmänvalvojan roskapostin vastaisessa käytännössä määrittämä sallittu lähettäjä tai toimialue.</span><span class="sxs-lookup"><span data-stu-id="af180-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="af180-113">Yhteyssuodatinkäytännön sallittu IP-osoite.</span><span class="sxs-lookup"><span data-stu-id="af180-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="af180-114">Postin kulkusääntö (jota kutsutaan myös siirtosäännöksi), joka on määritetty sallimaan viestit.</span><span class="sxs-lookup"><span data-stu-id="af180-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="af180-115">Jos uskot, että viesti on virheellisesti merkitty phish-merkinnäksi, lähetä viestiesimerkit Microsoftille [Outlookin raporttiviesti -apuohjelman](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) avulla.</span><span class="sxs-lookup"><span data-stu-id="af180-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
