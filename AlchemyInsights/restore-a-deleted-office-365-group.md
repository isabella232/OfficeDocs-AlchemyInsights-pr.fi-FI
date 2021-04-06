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
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597440"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="29a37-102">Poistetun Microsoft 365 -ryhmän palauttaminen</span><span class="sxs-lookup"><span data-stu-id="29a37-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="29a37-103">Voit palauttaa poistetun Microsoft 365 -ryhmän tai Microsoft Teamsin 30 päivän kuluessa poistamisesta.</span><span class="sxs-lookup"><span data-stu-id="29a37-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="29a37-104">Siirry [Microsoft 365 -hallintakeskukseen ja kirjaudu](https://aka.ms/RestoreDeletedGroup) sisään ja luetella poistetut ryhmät ja tiimit.</span><span class="sxs-lookup"><span data-stu-id="29a37-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in and list the deleted groups and teams.</span></span>

    <span data-ttu-id="29a37-105">**Huomautus:** Kirjaudu sisään käyttämällä tiliä, joka on määritetty joko vuokraajan järjestelmänvalvojalle tai ryhmien järjestelmänvalvojan roolille.</span><span class="sxs-lookup"><span data-stu-id="29a37-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="29a37-106">Valitse poistettu Microsoft 365 -ryhmä/Teams palautettavaksi ja valitse **Palauta ryhmä**.</span><span class="sxs-lookup"><span data-stu-id="29a37-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="29a37-107">Jos ryhmää ei voi palauttaa ristiriitaisten SMTP-osoitteiden vuoksi, etsi ristiriitaa aiheuttava objekti seuraavan komennon avulla ja poista SMTP-osoite:</span><span class="sxs-lookup"><span data-stu-id="29a37-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="29a37-108">**Huomautus:** Joissakin tapauksissa voi kestää jopa 24 tuntia, ennen kuin ryhmä ja kaikki sen tiedot palautetaan.</span><span class="sxs-lookup"><span data-stu-id="29a37-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="29a37-109">Lisätietoja tai lisätietoja ryhmien palauttamisesta PowerShellin avulla on kohdassa [Poistetun Microsoft 365 -ryhmän palauttaminen.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="29a37-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>