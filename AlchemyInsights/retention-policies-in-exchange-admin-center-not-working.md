---
title: Exchange-hallintakeskuksen säilytyskäytännöt eivät toimi
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952225"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="2b01e-102">Exchange-hallintakeskuksen säilytyskäytännöt</span><span class="sxs-lookup"><span data-stu-id="2b01e-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="2b01e-103">Jos haluat, että suoritamme automaattiset tarkistukset alla mainittujen asetusten varalta, valitse Sivun yläreunassa Takaisin-painike < ja kirjoita sitten sen käyttäjän sähköpostiosoite, jolla on ongelmia säilytyskäytäntöjen kanssa.</span><span class="sxs-lookup"><span data-stu-id="2b01e-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="2b01e-104">Jos Exchange-hallintakeskuksessa on säilytyskäytäntöjä, jotka eivät koske postilaatikoita tai kohteita, jotka eivät siirry arkistopostilaatikkoon, tarkista seuraavat asiat:</span><span class="sxs-lookup"><span data-stu-id="2b01e-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="2b01e-105">**Perimmäinen syy:**</span><span class="sxs-lookup"><span data-stu-id="2b01e-105">**Root Causes:**</span></span>

- <span data-ttu-id="2b01e-106">**Kansion hallinta -avustaja** ei ole käsitellyt käyttäjän postilaatikkoa.</span><span class="sxs-lookup"><span data-stu-id="2b01e-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="2b01e-107">Hallitun kansion avustaja yrittää käsitellä pilvipohjaisen organisaation jokaista postilaatikkoa seitsemän päivän välein.</span><span class="sxs-lookup"><span data-stu-id="2b01e-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="2b01e-108">**Ratkaisu:** Suorita Kansion hallinta -avustaja.</span><span class="sxs-lookup"><span data-stu-id="2b01e-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="2b01e-109">**RetentionHold** on **otettu** käyttöön postilaatikossa.</span><span class="sxs-lookup"><span data-stu-id="2b01e-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="2b01e-110">Jos postilaatikko on sijoitettu RetentionHold-kohteelle, postilaatikon säilytyskäytäntöä ei käsitellä kyseisenä aikana.</span><span class="sxs-lookup"><span data-stu-id="2b01e-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="2b01e-111">**Ratkaisu:** Tarkista säilytysten pitoasetuksen tila ja päivitä se tarvittaessa.</span><span class="sxs-lookup"><span data-stu-id="2b01e-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="2b01e-112">Lisätietoja on kohdassa [Postilaatikon säilytys .](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)</span><span class="sxs-lookup"><span data-stu-id="2b01e-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="2b01e-113">**Huomautus:** Jos postilaatikon koko on alle 10 Mt, Kansion hallinta -avustaja ei käsittele postilaatikkoa automaattisesti.</span><span class="sxs-lookup"><span data-stu-id="2b01e-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="2b01e-114">Lisätietoja Exchange-hallintakeskuksen säilytyskäytännöistä on kohdassa:</span><span class="sxs-lookup"><span data-stu-id="2b01e-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="2b01e-115">Säilytystunnisteet ja säilytyskäytännöt</span><span class="sxs-lookup"><span data-stu-id="2b01e-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="2b01e-116">[Säilytyskäytännön käyttäminen postilaatikoissa tai](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) [Säilytystunnisteiden lisääminen tai poistaminen](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="2b01e-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="2b01e-117">Postilaatikon pitotyypin tunnistaminen</span><span class="sxs-lookup"><span data-stu-id="2b01e-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
