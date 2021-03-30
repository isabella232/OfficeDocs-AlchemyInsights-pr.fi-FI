---
title: Azure Active Directoryn yhdistelmäliittämän vianmääritys
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401904"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Azure Active Directoryn yhdistelmäliittämän vianmääritys

Erittäin suositeltavaa: varmista, että laite voi käyttää järjestelmätilin laiterekisteröinnin päätepisteitä käyttämällä komentosarjaa [Testaa laiterekisteröinnin yhteyttä](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. Jos määrität laiterekisteröintiä ensimmäistä kertaa, muista tarkistaa [Johdanto Azure Active Directoryn laitehallintaan](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/), jotta saat lisätietoja laitteiden hallinnasta Azure AD:ssä.
1. Jos rekisteröit laitteita suoraan Azure Active Directoryyn ja kirjaat ne Intuneen, varmista ensin, että olet [määrittänyt Intunen](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) ja että [käyttöoikeudet](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) ovat kunnossa.
1. Varmista, että sinulla on oikeus suorittaa toimintoja Azure AD:ssä ja paikallisessa AD:ssä. Vain Azure AD:n yleinen järjestelmänvalvoja voi hallita laiterekisteröinnin asetuksia. Lisäksi jos määrität automaattisia rekisteröintejä paikalliseen Active Directoryyn, sinun on oltava Active Directoryn ja AD FS:n järjestelmänvalvoja (jos sovellettavissa).

Lisätietoja yhdistelmäliittämän mahdollisten ongelmien ratkaisemisesta on kohdassa [Yhdistelmäliittämän vianmääritys](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current); lisätietoja Azure AD:n yhdistelmäliittämän määrittämisestä ja laitteiden hallinnasta Azure AD -portaalissa on kohdissa [Azure AD:n yhdistelmäliittämän laitteiden määrittäminen (paikalliseen toimialueeseen liitetyt)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) ja [Laitteiden hallinta Azure-portaalissa](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Ratkaisuja yleisiin Azure Active Directoryn yhdistelmäliittämän ongelmiin on kohdassa [Azure AD:n yhdistelmäliittämän usein kysytyt kysymykset](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
