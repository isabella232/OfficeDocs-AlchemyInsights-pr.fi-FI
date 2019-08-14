---
title: 2491 ilmoitus sähköpostiviestit Phish toimitetaan vuokralaisen tai käyttäjän korvaa käytännön
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391244"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="3c3ab-102">Ilmoitus sähköpostiviestit Phish toimitetaan vuokralaisen tai käyttäjän korvaa käytännön</span><span class="sxs-lookup"><span data-stu-id="3c3ab-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="3c3ab-103">Oletusarvon mukainen ilmoitus käytännön nimeltä ”käyttäjän tai vuokralaisen ohituksen vuoksi Phish toimitettu” on on rullattu vuokralaiset käyttöoikeudet Office 365-ATP-P1 ja P2.</span><span class="sxs-lookup"><span data-stu-id="3c3ab-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="3c3ab-104">Jos olet saanut ilmoituksen, tässä on vaiheita voit tutkia:</span><span class="sxs-lookup"><span data-stu-id="3c3ab-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="3c3ab-105">Varoitussanoma klikkaa **Näytä ilmoitus** Go to Security & Compliance Centeriin **ilmoitukset** -sivulle.</span><span class="sxs-lookup"><span data-stu-id="3c3ab-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="3c3ab-106">Valitse **näkymässä viestiluettelon** tai **Resurssienhallinnan Näytä viestit**näet ilmoituksen.</span><span class="sxs-lookup"><span data-stu-id="3c3ab-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="3c3ab-107">Nämä asetukset löytyvät tiedot viestin, joka sisältää sanoman tunnus.</span><span class="sxs-lookup"><span data-stu-id="3c3ab-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="3c3ab-108">Huomaa, että uhka Explorer-linkin suodattaa automaattisesti ilmoituksen ehdot täyttävät viestit.</span><span class="sxs-lookup"><span data-stu-id="3c3ab-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="3c3ab-109">Uhka Explorerissa Pvm-suodatus on ehkä muutettava.</span><span class="sxs-lookup"><span data-stu-id="3c3ab-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="3c3ab-110">Tietojen kalastelu-viesti toimitettiin manuaalisesti määritetty ohituksen vuoksi:</span><span class="sxs-lookup"><span data-stu-id="3c3ab-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="3c3ab-111">Sallittu lähettäjän tai toimialueen käyttäjän määrittämä.</span><span class="sxs-lookup"><span data-stu-id="3c3ab-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="3c3ab-112">Sallittu lähettäjän tai toimialueen admin Anti-Spam-käytännön mukaan.</span><span class="sxs-lookup"><span data-stu-id="3c3ab-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="3c3ab-113">Sallittu käytännössä yhteyden suodattimen IP-osoite.</span><span class="sxs-lookup"><span data-stu-id="3c3ab-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="3c3ab-114">Postin kulkua sääntö (tunnetaan myös nimellä liikenteen sääntö), joka on määritetty sallimaan viestien.</span><span class="sxs-lookup"><span data-stu-id="3c3ab-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="3c3ab-115">Jos viesti on merkitty virheellisesti kalastella, Outlookin avulla [raporttisanoma apuohjelma](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) lähettää viestin Microsoft näytteiden.</span><span class="sxs-lookup"><span data-stu-id="3c3ab-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
