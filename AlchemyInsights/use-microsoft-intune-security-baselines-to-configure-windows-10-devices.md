---
title: Windows 10 -laitteiden määrittäminen Microsoft Intunen perusaikataulujen avulla
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50694430"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="d259a-102">Microsoft Intune -suojauksen perusaikataulujen käyttäminen Windows 10 -laitteiden määrittämiseen</span><span class="sxs-lookup"><span data-stu-id="d259a-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="d259a-103">Intune-suojauksen perusaikataulut auttavat suojaamaan käyttäjiä ja laitteita.</span><span class="sxs-lookup"><span data-stu-id="d259a-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="d259a-104">Suojauksen perusaikataulut ovat Windowsin asetusten ennalta määritettyjä ryhmiä, joiden avulla käytetään tunnettua asetus- ja oletusarvoryhmää, jota asianomaiset suojausryhmät suosittelevat.</span><span class="sxs-lookup"><span data-stu-id="d259a-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="d259a-105">Luomalla suojauksen perusaikataulun profiilin Intunessa luot mallin, joka koostuu useista laitemääritysprofiileista.</span><span class="sxs-lookup"><span data-stu-id="d259a-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="d259a-106">Kun otat suojauksen perusaikataulut käyttöön käyttäjä- tai laiteryhmissä, asetukset otetaan käyttöön laitteissa, jotka suoritetaan Windows 10:ssä tai sitä uudemmassa versiossa.</span><span class="sxs-lookup"><span data-stu-id="d259a-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="d259a-107">Esimerkiksi Microsoft mobile device management (MDM) -suojauksen perusaikataulu (1) ottaa BitLockerin käyttöön siirrettäville asemille (2) edellyttää salasanan laitteen lukituksen avaamista varten ja (3) poistaa perustodennuksen käytöstä.</span><span class="sxs-lookup"><span data-stu-id="d259a-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="d259a-108">Jos oletusarvo ei toimi ympäristössäsi, voit mukauttaa perusaikataulua haluamallasi asetuksilla.</span><span class="sxs-lookup"><span data-stu-id="d259a-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="d259a-109">Suojauksen perusaikataulut auttavat myös muodostamaan lopusta päähän -suojatun työnkulun Microsoft 365:ssä.</span><span class="sxs-lookup"><span data-stu-id="d259a-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="d259a-110">Seuraavassa on joitakin tämän toiminnon etuja:</span><span class="sxs-lookup"><span data-stu-id="d259a-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="d259a-111">Suojauksen perusaikataulu sisältää parhaat käytännöt ja suositukset tietoturvaan vaikuttavia asetuksia varten.</span><span class="sxs-lookup"><span data-stu-id="d259a-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="d259a-112">Koska Intune-kumppanit Windowsin suojaustiimin kanssa luovat perusaikatauluja ryhmäkäytäntöjä varten, nämä suositukset perustuvat vankkaihin ohjeisiin ja laajaan käyttökokemukseen.</span><span class="sxs-lookup"><span data-stu-id="d259a-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="d259a-113">Jos et ole ennen luonut Intunea etkä ole varma, mistä aloittaa, suojauksen perusaikataulujen avulla voit luoda ja ottaa käyttöön suojatun profiilin nopeasti.</span><span class="sxs-lookup"><span data-stu-id="d259a-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="d259a-114">Jos käytät tällä hetkellä ryhmäkäytäntöä, siirtyminen Intuneen hallintaa varten on huomattavasti helpompaa suojauksen perusaikataulujen avulla, koska nämä suojauksen perusaikataulut sisältyvät Intuneen ja sisältävät hallinnan huippuominaisuuksia.</span><span class="sxs-lookup"><span data-stu-id="d259a-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="d259a-115">Lisätietoja on ohjeaiheessa Windowsin suojauksen [perusaikataulut ja](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) [mobiililaitteiden hallinta.](https://docs.microsoft.com/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="d259a-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>