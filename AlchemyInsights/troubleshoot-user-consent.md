---
title: Käyttäjän suostumuksen vianmääritys
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901193"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="51b46-102">Käyttäjän suostumuksen vianmääritys</span><span class="sxs-lookup"><span data-stu-id="51b46-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="51b46-103">Voit määrittää, miten loppukäyttäjät hyväksyvät sovellukset Azure-portaalin tai PowerShellin kautta.</span><span class="sxs-lookup"><span data-stu-id="51b46-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="51b46-104">Lisätietoja [on käyttäjän suostumusasetuksissa.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings)</span><span class="sxs-lookup"><span data-stu-id="51b46-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="51b46-105">Järjestelmänvalvoja voi myös microsoft [Graph -ohjelmointirajapinnan](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) avulla myöntää suostumuksen delegoiduille käyttöoikeuksille yksittäisen käyttäjän puolesta.</span><span class="sxs-lookup"><span data-stu-id="51b46-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="51b46-106">Lisätietoja on kohdassa [Käytön saaminen käyttäjän puolesta.](https://docs.microsoft.com/graph/auth-v2-user)</span><span class="sxs-lookup"><span data-stu-id="51b46-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="51b46-107">[Käyttäjän suostumusvirheet:](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)tässä artikkelissa käsitellään virheitä, joita sovelluksen suostumuksen antamisen aikana voi ilmetä.</span><span class="sxs-lookup"><span data-stu-id="51b46-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="51b46-108">Jos suoritat vianmäärityksen odottamattomia suostumuskehotteita, jotka eivät sisällä virhesanomia, tutustu [Azure AD:n todennusskenaarioihin.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)</span><span class="sxs-lookup"><span data-stu-id="51b46-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>