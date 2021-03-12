---
title: Replikointijoukko
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/10/2021
ms.locfileid: "50713748"
---
# <a name="replica-set"></a><span data-ttu-id="8b899-102">Replikointijoukko</span><span class="sxs-lookup"><span data-stu-id="8b899-102">Replica set</span></span>

<span data-ttu-id="8b899-103">AADDS tunnetaan myös hallituna toimialueena.</span><span class="sxs-lookup"><span data-stu-id="8b899-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="8b899-104">Se on itse asiassa kaksi toimialueen ohjauskonetta, joita taustaohjain suorittaa ja ylläpitää.</span><span class="sxs-lookup"><span data-stu-id="8b899-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="8b899-105">Nämä kaksi DCs-tietokonetta sisältävät yhden dc:n päätietokoneen ja yhden replikoinnin DC:n.</span><span class="sxs-lookup"><span data-stu-id="8b899-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="8b899-106">Varmuuskopiot AADDS:ssä (hallittu toimialue) ovat Azure-ympäristön hallitsemia automaattisia prosessia.</span><span class="sxs-lookup"><span data-stu-id="8b899-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="8b899-107">Jos hallittuun toimialueeseen liittyy ongelma, Azuren tuki auttaa sinua palauttamaan tiedot varmuuskopioista.</span><span class="sxs-lookup"><span data-stu-id="8b899-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="8b899-108">Jokainen replikointijoukko luodaan virtuaalisessa verkossa.</span><span class="sxs-lookup"><span data-stu-id="8b899-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="8b899-109">Kunkin virtuaalisen verkoston on oltava vertaisverkko kaikissa muissa virtuaaliverkoissa, joissa isännöidä hallitun toimialueen replikointijoukkoa.</span><span class="sxs-lookup"><span data-stu-id="8b899-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="8b899-110">Tämä määritys luo verkkotopologian, joka tukee hakemiston replikointia.</span><span class="sxs-lookup"><span data-stu-id="8b899-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="8b899-111">Virtuaalinen verkko voi tukea useita replikointijoukkoja, jos kukin replikointijoukko on eri virtuaalisessa aliverkossa.</span><span class="sxs-lookup"><span data-stu-id="8b899-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="8b899-112">Lisätietoja replikointijoukosta on konseptien [replikointijoukoissa.](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)</span><span class="sxs-lookup"><span data-stu-id="8b899-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
