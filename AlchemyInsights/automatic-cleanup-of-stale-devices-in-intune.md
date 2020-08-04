---
title: Automaattinen puhdistus tunkkainen laitteiden Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554966"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="9b0dd-102">Automaattinen puhdistus tunkkainen laitteiden Intune</span><span class="sxs-lookup"><span data-stu-id="9b0dd-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="9b0dd-103">Intune antaa admin jotta configure aikaväliväliväli 90 ja 270 days, jonka jälkeen tunkkainen laitteet poistetaan palvelusta.</span><span class="sxs-lookup"><span data-stu-id="9b0dd-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="9b0dd-104">Tämä asetus on organisaation laajuinen ja kun aktivoitu, se tulee voimaan välittömästi.</span><span class="sxs-lookup"><span data-stu-id="9b0dd-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="9b0dd-105">Laitteet, joita ei ole kuitattu Intune-palvelimeen asetuksen ylittäväksi ajaksi, poistetaan pysyvästi.</span><span class="sxs-lookup"><span data-stu-id="9b0dd-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="9b0dd-106">**Huomautus** Vain MDM-laiteobjektit ovat oikeutettuja tähän puhdistustoimintoon.</span><span class="sxs-lookup"><span data-stu-id="9b0dd-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="9b0dd-107">EAS:lle jää vain laiteobjektit pois.</span><span class="sxs-lookup"><span data-stu-id="9b0dd-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="9b0dd-108">Lisätietoja siitä, milloin laite voidaan poistaa laitteen puhdistusasetuksen ja sen "tilan" perusteella:</span><span class="sxs-lookup"><span data-stu-id="9b0dd-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="9b0dd-109">Asetus: **Poista laitteet viimeisen sisäänkirjautumispäivän jälkeen: Kyllä (jokin arvo (N) määritettyinä päivinä)**</span><span class="sxs-lookup"><span data-stu-id="9b0dd-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="9b0dd-110">Intune-palvelu poistaa laitteen määritettyinä päivinä sen jälkeen, kun se on viimeksi kirjautunut sisään, arvon (N) perusteella.</span><span class="sxs-lookup"><span data-stu-id="9b0dd-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="9b0dd-111">Asetus: **Poista laitteet viimeisen sisäänkirjautumispäivän jälkeen: Ei**</span><span class="sxs-lookup"><span data-stu-id="9b0dd-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="9b0dd-112">180 päivän kuluttua laitteen varmenteen vanhenemisen päättymisestä eikä sitä uusita, laite poistetaan.</span><span class="sxs-lookup"><span data-stu-id="9b0dd-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="9b0dd-113">**Huomautus** Molemmissa tapauksissa laite on rekisteröitävä onnistuneesti Intunessa.</span><span class="sxs-lookup"><span data-stu-id="9b0dd-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="9b0dd-114">Rekisteröinti tapahtuu ensimmäisen laitetarkastuksen aikana Intune-palvelussa.</span><span class="sxs-lookup"><span data-stu-id="9b0dd-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="9b0dd-115">Jos laite rekisteröityy intuneen, mutta ei rekisteröi sitä, laite poistetaan 270 päivän kuluttua rekisteröitymisestä.</span><span class="sxs-lookup"><span data-stu-id="9b0dd-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="9b0dd-116">(90 päivää, jos haluat merkitä laitteen kumotuksi, ja sitten vielä 180 päivää tietueen poistamiseen.)</span><span class="sxs-lookup"><span data-stu-id="9b0dd-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="9b0dd-117">Intune-konsolissa ei ole tällä hetkellä mekanismia laitteen sertifioinnin vanhenemispäivän määrittämiseksi millekään laitteelle.</span><span class="sxs-lookup"><span data-stu-id="9b0dd-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>