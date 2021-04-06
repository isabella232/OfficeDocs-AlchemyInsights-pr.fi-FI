---
title: Officen ja OneDriven asentaminen Windowsin virtuaalityöpöydälle
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595623"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>Officen ja OneDriven asentaminen Windowsin virtuaalityöpöydälle

1. [Valmistele ja mukauta VHD-perustyylin kuva.](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image) Luo virtuaalikone (VM), jos sitä ei ole jo luotu.

1. [Asenna Office jaetun tietokoneen aktivointitilaan.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode) Jaetun tietokoneen aktivoinnin avulla useat käyttäjät voivat käyttää Officea.

1. [Asenna OneDrive kone kerrallaan.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode) OneDrive asennetaan yleensä käyttäjää kohti, mutta tässä se on asennettava konetta kohti.