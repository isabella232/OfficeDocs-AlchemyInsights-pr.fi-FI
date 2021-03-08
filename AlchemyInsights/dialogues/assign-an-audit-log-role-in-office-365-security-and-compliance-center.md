---
title: Valvontalokin roolin määrittäminen Office 365:n & yhteensopivuuskeskuksessa
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524791"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="bf36c-102">Valvontalokin roolin määrittäminen Office 365:n & yhteensopivuuskeskuksessa</span><span class="sxs-lookup"><span data-stu-id="bf36c-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="bf36c-103">Office 365:n valvontalokista hakeminen edellyttää, että järjestelmänvalvojalle on  määritetty Vain tarkasteleminen -valvontalokien rooli tai Valvontalokit-rooli Exchange Onlinessa. </span><span class="sxs-lookup"><span data-stu-id="bf36c-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="bf36c-104">Nämä roolit määritetään oletusarvoisesti yhteensopivuuden hallinnan ja organisaation hallinnan rooliryhmille.</span><span class="sxs-lookup"><span data-stu-id="bf36c-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="bf36c-105">Office 365:n ja Microsoft 365:n yleiset järjestelmänvalvojat lisätään automaattisesti Organisaation hallinta -rooliryhmän jäseniksi.</span><span class="sxs-lookup"><span data-stu-id="bf36c-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="bf36c-106">Jotta käyttäjä voi hakea mahdollisimman vähän käyttöoikeuksia, luo mukautettu rooliryhmä Exchange Onlinessa, lisää Vain  luku -valvontalokien rooli tai Valvontalokit-rooli ja lisää sitten käyttäjä uuden rooliryhmän jäseneksi. </span><span class="sxs-lookup"><span data-stu-id="bf36c-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="bf36c-107">Lisätietoja on kohdassa Rooliryhmien [hallinta Exchange Onlinessa](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) ja valvontalokista hakeminen [tietoturva- & yhteensopivuuskeskuksessa.](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)</span><span class="sxs-lookup"><span data-stu-id="bf36c-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>