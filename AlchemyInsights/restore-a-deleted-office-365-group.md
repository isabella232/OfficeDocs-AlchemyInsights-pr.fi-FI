---
title: Poistetun Microsoft 365 -ryhmän palauttaminen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6f640093cd099f20d3a95eede5c141ad74838b0b
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505683"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="ca1c4-102">Poistetun Microsoft 365 -ryhmän palauttaminen</span><span class="sxs-lookup"><span data-stu-id="ca1c4-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="ca1c4-103">Voit palauttaa poistetun Microsoft 365 -ryhmän tai Microsoft Teamsin 30 päivän kuluessa poistamisesta.</span><span class="sxs-lookup"><span data-stu-id="ca1c4-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="ca1c4-104">Jos haluat kirjautua Microsoft 365 -hallintakeskukseen ja luetella poistetut ryhmät ja ryhmät, siirry [Microsoft 365 -hallintakeskukseen.](https://aka.ms/RestoreDeletedGroup)</span><span class="sxs-lookup"><span data-stu-id="ca1c4-104">To login to Microsoft 365 admin center and list the deleted groups and teams, go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup).</span></span>

    <span data-ttu-id="ca1c4-105">**Huomautus:** Kirjaudu sisään käyttämällä tiliä, joka on määritetty joko vuokraajan järjestelmänvalvojalle tai ryhmien järjestelmänvalvojan roolille.</span><span class="sxs-lookup"><span data-stu-id="ca1c4-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="ca1c4-106">Valitse palautettava poistettu Microsoft 365 -ryhmä tai Teams ja valitse **palauta ryhmä.**</span><span class="sxs-lookup"><span data-stu-id="ca1c4-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="ca1c4-107">Jos ryhmää ei voi palauttaa ristiriitaisten SMTP-osoitteiden vuoksi, etsi ristiriitaa aiheuttava objekti seuraavan komennon avulla ja poista SMTP-osoite:</span><span class="sxs-lookup"><span data-stu-id="ca1c4-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="ca1c4-108">**Huomautus:** Joissakin tapauksissa voi kestää jopa 24 tuntia, ennen kuin ryhmä ja kaikki sen tiedot palautetaan.</span><span class="sxs-lookup"><span data-stu-id="ca1c4-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="ca1c4-109">Lisätietoja tai tietoja ryhmien palauttamisesta PowerShellin avulla on ohjeaiheessa [Poistetun Microsoft 365 -ryhmän palauttaminen.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="ca1c4-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>