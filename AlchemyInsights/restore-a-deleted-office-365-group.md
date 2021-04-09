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
ms.openlocfilehash: b72b7c93ce9fe1b90d1608811b0eeabc8aec1363
ms.sourcegitcommit: a5edaaefdc56f8d5c8220a335f4e8228e2de4ee0
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/08/2021
ms.locfileid: "51645128"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="49c56-102">Poistetun Microsoft 365 -ryhmän palauttaminen</span><span class="sxs-lookup"><span data-stu-id="49c56-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="49c56-103">Voit palauttaa poistetun Microsoft 365 -ryhmän tai Microsoft Teamsin 30 päivän kuluessa poistamisesta.</span><span class="sxs-lookup"><span data-stu-id="49c56-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="49c56-104">Siirry [Microsoft 365 -hallintakeskukseen](https://aka.ms/RestoreDeletedGroup) ja kirjaudu sisään luetteloon, jossa näet, että olet poistetut ryhmät ja tiimit.</span><span class="sxs-lookup"><span data-stu-id="49c56-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in to a list of your the deleted groups and teams.</span></span>

    <span data-ttu-id="49c56-105">**Huomautus:** Kirjaudu sisään käyttämällä tiliä, joka on määritetty joko vuokraajan järjestelmänvalvojalle tai ryhmien järjestelmänvalvojan roolille.</span><span class="sxs-lookup"><span data-stu-id="49c56-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="49c56-106">Valitse poistettu Microsoft 365 -ryhmä/Teams palautettavaksi ja valitse **Palauta ryhmä**.</span><span class="sxs-lookup"><span data-stu-id="49c56-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="49c56-107">Jos ryhmää ei voi palauttaa ristiriitaisten SMTP-osoitteiden vuoksi, etsi ristiriitaa aiheuttava objekti seuraavan komennon avulla ja poista SMTP-osoite:</span><span class="sxs-lookup"><span data-stu-id="49c56-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="49c56-108">**Huomautus:** Joissakin tapauksissa voi kestää jopa 24 tuntia, ennen kuin ryhmä ja kaikki sen tiedot palautetaan.</span><span class="sxs-lookup"><span data-stu-id="49c56-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="49c56-109">Lisätietoja tai lisätietoja ryhmien palauttamisesta PowerShellin avulla on kohdassa [Poistetun Microsoft 365 -ryhmän palauttaminen.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="49c56-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>