---
title: Käyttäjän määrittämän hallitun käyttäjätietojen hallinta
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8211"
- "9003230"
ms.openlocfilehash: a44cb484b6d89e6d5f67b2900c38dde3610b0e23
ms.sourcegitcommit: 23e778f7414e5f1a98cc786146fe76d622b458bc
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177577"
---
# <a name="manage-a-user-assigned-managed-identity"></a><span data-ttu-id="d8d25-102">Käyttäjän määrittämän hallitun käyttäjätietojen hallinta</span><span class="sxs-lookup"><span data-stu-id="d8d25-102">Manage a user-assigned managed identity</span></span>

<span data-ttu-id="d8d25-103">Käyttäjälle määritettyjen hallittujen käyttäjätietojen hallintaan kuuluu:</span><span class="sxs-lookup"><span data-stu-id="d8d25-103">The management of a user-assigned managed identity involves:</span></span>

- <span data-ttu-id="d8d25-104">Roolien määrittäminen käyttäjälle määritetyille hallituille käyttäjätiimeille</span><span class="sxs-lookup"><span data-stu-id="d8d25-104">Assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="d8d25-105">Käyttäjän määrittämän hallitun käyttäjätietojen poistaminen</span><span class="sxs-lookup"><span data-stu-id="d8d25-105">Deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="d8d25-106">Käyttäjälle määritetyn hallitun käyttäjätietojen luettelo</span><span class="sxs-lookup"><span data-stu-id="d8d25-106">Listing a user-assigned managed identity</span></span>

<span data-ttu-id="d8d25-107">Lisätietoja edellä mainituista tehtävistä on seuraavissa artikkeleissa:</span><span class="sxs-lookup"><span data-stu-id="d8d25-107">For more information on the tasks mentioned above, see the following articles:</span></span>

- <span data-ttu-id="d8d25-108">[Käyttäjälle määritetyn hallitun käyttäjätietojen luominen](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) – roolien määrittäminen käyttäjälle määritetyille hallituille käyttäjätiimeille</span><span class="sxs-lookup"><span data-stu-id="d8d25-108">[How to create a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="d8d25-109">[Käyttäjälle määritetyn hallitun käyttäjätietojen poistaminen](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) – käyttäjälle määritetyn hallitun käyttäjätietojen poistaminen</span><span class="sxs-lookup"><span data-stu-id="d8d25-109">[How to delete a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="d8d25-110">[Käyttäjän määrittäjen hallittujen käyttäjätietojen luettelointi](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) – käyttäjän määrittämän hallitun käyttäjätietojen luetteloiminen</span><span class="sxs-lookup"><span data-stu-id="d8d25-110">[How to list a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for listing a user-assigned managed identity</span></span>

> [!NOTE]
> <span data-ttu-id="d8d25-111">Tarkista, onko sinulla hallittujen **käyttäjätietojen avustajaroolimääritys.**</span><span class="sxs-lookup"><span data-stu-id="d8d25-111">Verify whether you have the **Managed Identity Contributor** role assignment.</span></span> <span data-ttu-id="d8d25-112">Tämä roolimääritys tarvitaan käyttäjän määrittävien hallittujen käyttäjähenkilöllisyksien luomiseen ja poistamiseen.</span><span class="sxs-lookup"><span data-stu-id="d8d25-112">That role assignment is required for creating/deleting user-assigned managed identities.</span></span>
