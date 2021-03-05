---
title: MIM-synkronointipalvelun määrittäminen
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
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481352"
---
# <a name="configure-mim-sync-service"></a><span data-ttu-id="a6365-102">MIM-synkronointipalvelun määrittäminen</span><span class="sxs-lookup"><span data-stu-id="a6365-102">Configure MIM Sync service</span></span>

<span data-ttu-id="a6365-103">Microsoft Identity Manager (MIM) -synkronointipalvelu on MIM:n osa.</span><span class="sxs-lookup"><span data-stu-id="a6365-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="a6365-104">Se on keskitetty paikallinen palvelu, joka tallentaa ja integroi tietoja organisaatioille, joissa on useita paikallisia hakemistoja ja tietokantoja.</span><span class="sxs-lookup"><span data-stu-id="a6365-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="a6365-105">Voit ehkä ratkaista MIM Sync -ongelman, jos ongelma on ratkaistu MIM:n viimeisimmässä päivityksessä tai jossakin muissa alla olevassa osiossa mainituista ongelmista.</span><span class="sxs-lookup"><span data-stu-id="a6365-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="a6365-106">**Suositellut vaiheet**</span><span class="sxs-lookup"><span data-stu-id="a6365-106">**Recommended steps**</span></span>

1. <span data-ttu-id="a6365-107">Varmista, että käytät MIM Syncin viimeaikaista päivitystä, ja tarkista [MIM Syncin julkaisutiedot](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) ja selvitä, onko ongelma korjattu päivityksessä.</span><span class="sxs-lookup"><span data-stu-id="a6365-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="a6365-108">Jos ongelma liittyy Generic LDAP-, Generic SQL-, Lotus Domino- tai Web Services -yhdistimeen, varmista, että käytät yleisten yhdistimien [viimeaikaista päivitystä.](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)</span><span class="sxs-lookup"><span data-stu-id="a6365-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="a6365-109">Jos MIM-synkronointi suoritetaan, jossa on virhe, [](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) selvitä mahdolliset syyt suorita-virhekoodien taulukosta.</span><span class="sxs-lookup"><span data-stu-id="a6365-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="a6365-110">Jos run stops with **extension-dll-exception,** then click on those words to open the **Connector Space Object properties** window, and click on Stack **Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception.](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx)</span><span class="sxs-lookup"><span data-stu-id="a6365-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="a6365-111">Jos PCNS (Password Change Notification Service) -komponentti ilmoittaa virheestä **6025** tapahtumalokissa salasanasynkronoinnin aikana, tarkista [PCNS-raportointivirheen 6025 vianmääritys oppaasta.](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)</span><span class="sxs-lookup"><span data-stu-id="a6365-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="a6365-112">Jos täydellinen synkronointi FIM-palvelun hallintaagentin  kanssa on hidasta, tarkista TempDB:n automaattinen kasvu -asetus, joka on kuvattu kohdassa Täyden synkronoinnin vianmääritys tai koko synkronoinnin [riippuvan vianmäärityksen ohje.](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)</span><span class="sxs-lookup"><span data-stu-id="a6365-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="a6365-113">Jos kohtaat virheen, jossa pysäytetty palvelin ja epäonnistunut luominen www-palvelujen kautta FIM-palvelun hallintaagentin avulla, katso [tukitiedot: via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) -palveluiden kautta epäonnistunut luominen, jossa on yleiskuvaus syistä.</span><span class="sxs-lookup"><span data-stu-id="a6365-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

