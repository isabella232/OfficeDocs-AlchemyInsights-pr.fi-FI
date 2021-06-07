---
title: Perusaikataulujen Microsoft Intune määrittäminen laitteiden Windows 10 perusaikataulujen avulla
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793698"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="32f11-102">Perusaikataulujen Microsoft Intune määrittäminen laitteiden Windows 10 perusaikataulujen avulla</span><span class="sxs-lookup"><span data-stu-id="32f11-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="32f11-103">Intune-suojauksen perusaikataulut auttavat suojaamaan käyttäjiä ja laitteita.</span><span class="sxs-lookup"><span data-stu-id="32f11-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="32f11-104">Suojauksen perusaikataulut Windows ovat valmiiksi määritettyjä ryhmiä, joiden avulla sovelletaan tunnettuja asetuksia ja oletusarvoja, joita asianomaiset suojausryhmät suosittelevat.</span><span class="sxs-lookup"><span data-stu-id="32f11-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="32f11-105">Luomalla suojauksen perusaikataulun profiilin Intunessa voit luoda mallin, joka koostuu useista laitemääritysprofiileista.</span><span class="sxs-lookup"><span data-stu-id="32f11-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="32f11-106">Kun otat käyttöön suojauksen perusaikataulut käyttäjä- tai laiteryhmissä, asetukset otetaan käyttöön laitteissa, jotka suoritetaan Windows 10 uudemmassa.</span><span class="sxs-lookup"><span data-stu-id="32f11-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="32f11-107">Esimerkiksi Microsoftin mobiililaitteiden hallinnan suojauksen perusaikataulu mahdollistaa siirrettävien BitLocker automaattisen suojauksen, vaatii salasanan laitteen lukituksen poistamiseen ja poistaa perustodennuksen käytöstä.</span><span class="sxs-lookup"><span data-stu-id="32f11-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="32f11-108">Jos oletusarvo ei toimi ympäristössäsi, voit mukauttaa perusaikataulua tarvitsemallasi asetuksilla.</span><span class="sxs-lookup"><span data-stu-id="32f11-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="32f11-109">Suojauksen perusaikataulut auttavat myös luomaan lopusta loppuun suojatun työnkulun Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="32f11-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="32f11-110">Suojauksen perusaikataulu sisältää parhaat käytännöt ja suojausta koskevat asetukset.</span><span class="sxs-lookup"><span data-stu-id="32f11-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="32f11-111">Intune kumppanit Windows kanssa, joka luo perusaikatauluja ryhmäkäytäntöjä varten, joten nämä suositukset perustuvat vankkaan ohjeeseen ja laajaan käyttökokemukseen.</span><span class="sxs-lookup"><span data-stu-id="32f11-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="32f11-112">Jos et ole ennen luonut Intunea etkä tiedä, mistä aloittaa, suojauksen perusaikataulujen avulla voit luoda ja ottaa käyttöön suojatun profiilin nopeasti.</span><span class="sxs-lookup"><span data-stu-id="32f11-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="32f11-113">Jos käytät tällä hetkellä ryhmäkäytäntöä, siirtyminen Intuneen hallintatarkoituksiin on huomattavasti helpompaa suojauksen perusaikataulujen avulla, koska ne sisältyvät Intuneen ja sisältävät huipputason hallintaominaisuuksia.</span><span class="sxs-lookup"><span data-stu-id="32f11-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="32f11-114">Lisätietoja on ohjeaiheessa Windows [perusaikataulut ja](/windows/security/threat-protection/windows-security-baselines) [mobiililaitteiden hallinta.](/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="32f11-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

