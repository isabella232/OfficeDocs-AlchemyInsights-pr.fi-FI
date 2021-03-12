---
title: 1:1-puhelutallenne
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733846"
---
# <a name="11-call-recording"></a><span data-ttu-id="f451e-102">1:1-puhelutallenne</span><span class="sxs-lookup"><span data-stu-id="f451e-102">1:1 call recording</span></span>

<span data-ttu-id="f451e-103">Järjestelmänvalvojien on nyt jatkettava 1:1-puheluiden tallentamista.</span><span class="sxs-lookup"><span data-stu-id="f451e-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="f451e-104">12. huhtikuuta 2021 alkaen otamme käyttöön uuden Teams-puhelukäytäntövaihtoehdon *AllowCloudRecordingForCalls.*</span><span class="sxs-lookup"><span data-stu-id="f451e-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="f451e-105">Tällä hetkellä yhden puhelun tallennusominaisuuksia hallitaan Teamsin *kokouskäytäntöjen AllowCloudRecording-vaihtoehdolla.*</span><span class="sxs-lookup"><span data-stu-id="f451e-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="f451e-106">Jos käyttäjät voivat tallentaa Teams-kokouksia, he voivat myös tallentaa 1:1-puheluita.</span><span class="sxs-lookup"><span data-stu-id="f451e-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="f451e-107">Jos haluat estää kaikkia käyttäjiä nauhoittamaan 1:1-puheluita, sinun ei tarvitse tehdä mitään.</span><span class="sxs-lookup"><span data-stu-id="f451e-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="f451e-108">*AllowCloudRecordingForCalls-puhelukäytäntöasetus* $False oletusarvoisesti.</span><span class="sxs-lookup"><span data-stu-id="f451e-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="f451e-109">Tämä muutos on dokumentoitu seuraavassa viestikeskuksen viestissä: [(Päivitetty) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) Puhelun tallennuskäytännön esittely Teams-puhelukäytäntövaihtoehdon valitsemiseen on käytettävä [Teams PowerShelliä.](https://docs.microsoft.com/microsoftteams/teams-powershell-install)</span><span class="sxs-lookup"><span data-stu-id="f451e-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="f451e-110">**Puhelutallenteen ottaminen käyttöön 1:1-puheluissa:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="f451e-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="f451e-111">**Puhelun tallennuksen poistaminen käytöstä 1:1-puheluissa:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span><span class="sxs-lookup"><span data-stu-id="f451e-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

