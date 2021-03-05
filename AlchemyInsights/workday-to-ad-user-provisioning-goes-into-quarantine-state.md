---
title: Työpäivä AD-käyttäjien valmisteluun siirtyy karanteeniin
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481357"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="37a42-102">Työpäivä AD-käyttäjien valmisteluun siirtyy karanteeniin</span><span class="sxs-lookup"><span data-stu-id="37a42-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="37a42-103">**Työpäivä AD-käyttäjien valmisteluun siirtyy karanteeniin eikä käyttäjiä luoda AD:ssä**</span><span class="sxs-lookup"><span data-stu-id="37a42-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="37a42-104">Työpäivä AD-käyttäjien valmistelutyö on mennyt karanteeniin, ja valvontalokeja käytettäessä näytetään vientivirhetapahtumat, joiden virhesanoma **on Virhe: OperationsError-SvcErr: Tapahtui toimintovirhe. Hakemistopalveluun ei ole määritetty parempia viittauksia. Hakemistopalvelu ei siis voi antaa suosituksia tämän metsän ulkopuolisille objekteille.**</span><span class="sxs-lookup"><span data-stu-id="37a42-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="37a42-105">Tämä virhe ilmenee yleensä, jos Active Directory -säilöä OU ei ole määritetty oikein tai jos **parentDistinguishedName-lausekkeen yhdistämismäärityksessä on ongelmia.**</span><span class="sxs-lookup"><span data-stu-id="37a42-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="37a42-106">Tarkista uusien käyttäjien oletus ou **-parametri** kirjoitusvirheiden tarkistaminen.</span><span class="sxs-lookup"><span data-stu-id="37a42-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="37a42-107">Varmista, että määritetty OU on jo ad-kentässä.</span><span class="sxs-lookup"><span data-stu-id="37a42-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="37a42-108">Jos käytät **parentDistinguishedName-nimeä** määritteiden yhdistämisessä, varmista, että se arvioi aina AD-toimialueen tunnetun säilön.</span><span class="sxs-lookup"><span data-stu-id="37a42-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="37a42-109">Tarkista valvontalokien Vie-tapahtuma, jotta näet luodun arvon.</span><span class="sxs-lookup"><span data-stu-id="37a42-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="37a42-110">Lisätietoja työpäivän määrittämisestä automaattista valmistelua varten on opetusohjelmassa: Työpäivän määrittäminen [automaattista käyttäjien valmistelua varten.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="37a42-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

