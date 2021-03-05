---
title: Valmistelupalvelun määrittäminen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/05/2021
ms.locfileid: "50481854"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="528bb-102">Valmistelupalvelun määrittäminen</span><span class="sxs-lookup"><span data-stu-id="528bb-102">Configuring the Provision service</span></span>

<span data-ttu-id="528bb-103">Jotta automaattinen käyttäjien valmistelu toimii, Azure AD edellyttää kelvollisia tunnistetietoja, joiden avulla se voi muodostaa yhteyden Työpäivä-verkkopalveluiden ohjelmointirajapintaan.</span><span class="sxs-lookup"><span data-stu-id="528bb-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="528bb-104">Lisäksi Työpäivä- ja AD-käyttäjien valmistelusovelluksen Testaa yhteyttä -painike vahvistaa myös, jos se pystyy muodostamaan yhteyden AD-toimialueeseen liittyvään Azure AD Connect -valmisteluedustajaan.</span><span class="sxs-lookup"><span data-stu-id="528bb-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="528bb-105">Jos Azure-portaali palauttaa virheilmoituksen tunnistetietojen tallentamisen yhteydessä, noudata seuraavia suositeltuja ohjeita:</span><span class="sxs-lookup"><span data-stu-id="528bb-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="528bb-106">Varmista, että olet määrittänyt Työpäivä-integroinnin järjestelmän käyttäjätilin opetusohjelman kohdassa Määritä [integrointijärjestelmän käyttäjä Työpäivässä.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="528bb-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="528bb-107">Varmista, että Azure AD Connect -valmisteluagenttipalvelu on käytössä paikallisella Windows-palvelimella palveluiden hallintakonsolin avulla.</span><span class="sxs-lookup"><span data-stu-id="528bb-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="528bb-108">Voit tarkistaa edustajan tilan myös Azure-portaalissa napsauttamalla Näytä paikalliset edustajat -painiketta.</span><span class="sxs-lookup"><span data-stu-id="528bb-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="528bb-109">Varmista, että kirjoitat Työpäivänimi-kentän arvon käyttämällä username@workday vuokraajan nimen muotoilua.</span><span class="sxs-lookup"><span data-stu-id="528bb-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="528bb-110">Jos työpäivä- ja vuokraajanimi puuttuu, Työpäivä-todennus epäonnistuu.</span><span class="sxs-lookup"><span data-stu-id="528bb-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="528bb-111">Jos olet määrittämässä integrointia Työpäivä-toteutuksen vuokraajan kanssa, ota huomioon Työpäivä-vuokraajan ajoitetut käyttökatkotunnit.</span><span class="sxs-lookup"><span data-stu-id="528bb-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="528bb-112">Työpäivä on ajoitettu käyttöajalta viikonloppuisin (yleensä perjantai-illasta lauantaiaamuun) ja yhteysongelmat tämän käyttökatkosikkunan aikana on tunnettu ongelma, joka korjaantuminen automaattisesti heti, kun toteutuksen vuokralaiset ovat taas online-tilassa.</span><span class="sxs-lookup"><span data-stu-id="528bb-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="528bb-113">Joissakin harvoissa tapauksissa saatat nähdä tämän virheen myös, jos integrointijärjestelmän käyttäjän salasana muuttuu vuokraajan päivityksen vuoksi tai jos tili on lukittuna tai vanhentunut.</span><span class="sxs-lookup"><span data-stu-id="528bb-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="528bb-114">Tarkista Integrointijärjestelmä-käyttäjän tila Työpäivä-järjestelmänvalvojalta.</span><span class="sxs-lookup"><span data-stu-id="528bb-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="528bb-115">Lisätietoja työpäivän määrittämisestä automaattista valmistelua varten on opetusohjelmassa: Työpäivän määrittäminen [automaattista käyttäjien valmistelua varten.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="528bb-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
