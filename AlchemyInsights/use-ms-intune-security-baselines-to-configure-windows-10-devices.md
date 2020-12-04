---
title: Windows 10-laitteiden määrittäminen Microsoft Intune-tieto turva perusaikataulujen avulla
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573400"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="f32ed-102">Windows 10-laitteiden määrittäminen Microsoft Intune-tieto turva perusaikataulujen avulla</span><span class="sxs-lookup"><span data-stu-id="f32ed-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="f32ed-103">Intune-suojaus perusaikataulujen avulla voit suojata käyttäjiä ja laitteita.</span><span class="sxs-lookup"><span data-stu-id="f32ed-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="f32ed-104">Tieto turvan perusaikataulut ovat Windowsin asetukset valmiiksi määritetyt ryhmät, joita käytetään tunnettujen tieto turva ryhmien suosittelemien asetus ryhmien ja oletus arvojen käyttöön.</span><span class="sxs-lookup"><span data-stu-id="f32ed-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="f32ed-105">Luomalla Intune-tieto turvan Perusprofiilin luot mallin, joka koostuu useista laite määritys profiileista.</span><span class="sxs-lookup"><span data-stu-id="f32ed-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="f32ed-106">Kun otat käyttöön tieto turvan perusviivat käyttäjien tai laitteiden ryhmille, asetukset otetaan käyttöön laitteissa, jotka toimivat Windows 10: ssä tai sitä uudemmissa versioissa.</span><span class="sxs-lookup"><span data-stu-id="f32ed-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="f32ed-107">Esimerkiksi MDM-tieto turvan perusaikataulu (1) mahdollistaa siirrettävien asemien BitLocker-Sala uksen, (2) edellyttää laitteen lukituksen poistamiseen ja (3) poistaa perustodennuksen käytöstä.</span><span class="sxs-lookup"><span data-stu-id="f32ed-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="f32ed-108">Kun oletus arvo ei toimi ympäristössäsi, Mukauta perusviivaa ja ota käyttöön tarvitsemasi asetukset.</span><span class="sxs-lookup"><span data-stu-id="f32ed-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="f32ed-109">Tieto turvan perusaikataulujen avulla voit myös määrittää end-to-end-suojatun työn kulun Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="f32ed-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="f32ed-110">Seuraavista eduista on hyötyä:</span><span class="sxs-lookup"><span data-stu-id="f32ed-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="f32ed-111">Tieto turvan perusaikataulu sisältää parhaita käytäntöjä ja suosituksia, jotka vaikuttavat tieto turvaan.</span><span class="sxs-lookup"><span data-stu-id="f32ed-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="f32ed-112">Koska Intune-kumppanit käyttävät Windowsin tieto turva tiimiä, joka luo perusaikatauluja ryhmä käytännöille, nämä suositukset perustuvat kiinteään ohja ukseen ja laajaan kokemukseen.</span><span class="sxs-lookup"><span data-stu-id="f32ed-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="f32ed-113">Jos olet uusi Intune-käyttäjä ja olet epävarma aloitus paikasta, voit luoda ja ottaa käyttöön suojatun profiilin nopeasti luomalla suojaus perusaikataulujen avulla.</span><span class="sxs-lookup"><span data-stu-id="f32ed-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="f32ed-114">Jos käytät tällä hetkellä ryhmä käytäntöä, siirtyminen Intune-järjestelmään hallinta tarkoituksissa on paljon helpompaa, koska ne on luotu Intune-käyttöön ja ne sisältävät hallinnan huippu ominaisuudet.</span><span class="sxs-lookup"><span data-stu-id="f32ed-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="f32ed-115">Lisä tietoja on artikkelissa [Windowsin tieto turvan perusviivat](https://go.microsoft.com/fwlink/?linkid=2141503) ja [mobiililaitteiden hallinta](https://go.microsoft.com/fwlink/?linkid=2141701).</span><span class="sxs-lookup"><span data-stu-id="f32ed-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>