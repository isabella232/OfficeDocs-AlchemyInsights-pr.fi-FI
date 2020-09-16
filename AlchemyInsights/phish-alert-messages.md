---
title: 2491-ilmoitukset Sähkö posti viesteistä, jotka on annettu vuokra ajan tai käyttäjän ohitus käytännöstä johtuen
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728608"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="6d351-102">Sähkö posti viestien ilmoitusten lähettäminen vuokra ajan tai käyttäjän ohitus käytännöstä johtuen</span><span class="sxs-lookup"><span data-stu-id="6d351-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="6d351-103">Oletusarvoiset ilmoitus käytännöt, joiden nimenä on "Phish Delivered vuokra ajan tai käyttäjän ohituksen takia", on otettu käyttöön vuokralaisille Office 365 ATP P1-ja P2-käyttö oikeuksien avulla</span><span class="sxs-lookup"><span data-stu-id="6d351-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="6d351-104">Jos sait tämän ilmoituksen, tutki seuraavat vaiheet:</span><span class="sxs-lookup"><span data-stu-id="6d351-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="6d351-105">Valitse ilmoitus viestistä **Näytä ilmoitus** , jos haluat siirtyä **ilmoitukset** -sivulle tieto turva-& yhteensopivuus keskuksessa.</span><span class="sxs-lookup"><span data-stu-id="6d351-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="6d351-106">Valitse ilmoitus, jos haluat tarkastella **viesti luetteloa** tai **tarkastella viestejä Resurssienhallinnassa**.</span><span class="sxs-lookup"><span data-stu-id="6d351-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="6d351-107">Molempien vaihto ehtojen avulla voit tarkastella viestin tietoja, kuten viestin tunnusta.</span><span class="sxs-lookup"><span data-stu-id="6d351-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="6d351-108">Huomaa, että Threat Explorer-linkki suodattaa automaattisesti ilmoitukset, jotka vastaavat ilmoitus ehtoja.</span><span class="sxs-lookup"><span data-stu-id="6d351-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="6d351-109">Sinun on ehkä muutettava päivämäärä suodatinta uhan hallinnassa.</span><span class="sxs-lookup"><span data-stu-id="6d351-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="6d351-110">Tietojenkalasteluviesti toimitettiin manuaalisesti määritetyn ohituksen takia:</span><span class="sxs-lookup"><span data-stu-id="6d351-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="6d351-111">Käyttäjä on määrittänyt sallitun lähettäjän tai toimi alueen.</span><span class="sxs-lookup"><span data-stu-id="6d351-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="6d351-112">Järjestelmänvalvoja on määrittänyt roska postin torjunta käytäntöön sallitun lähettäjän tai toimi alueen.</span><span class="sxs-lookup"><span data-stu-id="6d351-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="6d351-113">Sallittu IP-osoite yhteys suodatus käytännössä.</span><span class="sxs-lookup"><span data-stu-id="6d351-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="6d351-114">Sähkö postin kulku sääntö (jota kutsutaan myös siirto säännöksi), joka on määritetty sallimaan viestit-sovelluksessa.</span><span class="sxs-lookup"><span data-stu-id="6d351-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="6d351-115">Jos uskot, että viesti on merkitty virheellisesti Phish-muodossa, Lähetä viesti näytteitä Microsoftille Outlook- [raportti viesti-apuohjelman](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) avulla.</span><span class="sxs-lookup"><span data-stu-id="6d351-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
