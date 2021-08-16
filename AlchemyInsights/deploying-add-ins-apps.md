---
title: Apu in käyttöönotto Microsoft 365 -sovellukset
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: 3aacc3c6675f4102a5b34a435c862215dbfd0479b75549d608ed3c91021ed3d7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031403"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>Apu in käyttöönotto Microsoft 365 -sovellukset

Keskitetty käyttöönotto on suositeltava tapa ottaa käyttöön Office ja ryhmiä organisaation käyttäjille ja ryhmille. Ota apuohjelmat käyttöön noudattamalla seuraavia ohjeita:

**Huomautus:** Jos haluat asentaa apuohjelmat Office yksittäisenä käyttäjänä, katso Lisätietoja apuohjelmien tarkasteleminen, hallinta [ja asentaminen Office ohjelmissa.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) Varmista myös, että Office Storen apuohjelmat on otettu käyttöön. Lisätietoja on kohdassa [Apuohjelman latausten estäminen](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)ottamalla Office käytöstä kaikissa asiakasohjelmat (paitsi Outlook).

1. Varmista, että ympäristösi täyttää apuohjelmat käyttöönoton vaatimukset keskitetyn käyttöönoton avulla. Lisätietoja on kohdassa [Vaatimukset](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).
2. Siirry **Asetukset**  >  **integrated apps** Get  >  **apps** in the Microsoft 365 -hallintakeskus ja ota apuohjelmat käyttöön. 

Huomautukset: 

- Integroidut sovellukset edellyttävät, että järjestelmänvalvojalla on yleisen järjestelmänvalvojan Exchange järjestelmänvalvojan oikeudet.

- Kun apuohjelmat otetaan käyttöön useille käyttäjille, on suositeltavaa tehdä tehtäviä käyttämällä ryhmiä yksittäisten käyttäjien sijaan. Lisätietoja on kohdassa Huomioon [otettavia seikkoja, kun apuohjelma määritetään käyttäjille ja ryhmille.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)

- Keskitetty käyttöönotto ei tue sisäkkäisten ryhmien tai pääryhmien käyttäjiä. Lisätietoja on kohdassa [Käyttäjä- ja ryhmämääritykset.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)

- Varmista, että Microsoft 365 app management service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') on otettu käyttöön käyttäjille. Lisätietoja on kohdassa [Sovelluksen ominaisuuksien määrittäminen.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)

- Jos sinulla on ongelmia apuohjelmien käyttöönotossa integroitujen sovellusten avulla, kokeile käyttöönottoa [apuohjelmilla.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)

Lisätietoja on seuraavissa artikkeleissa:

[Apu in käyttöönotto hallintakeskuksessa](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Apu in hallintakeskuksessa](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Aputyökalujen hallinta keskitetyn käyttöönoton PowerShell-cmdlet-komentojen avulla](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Julkaise Office käyttämällä keskitettyä käyttöönottoa](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 Microsoft 365 -hallintakeskus [Vianmääritys: Käyttäjät eivät näe apu ins.](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Käyttäjävirheiden Office apuohjelmat](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)