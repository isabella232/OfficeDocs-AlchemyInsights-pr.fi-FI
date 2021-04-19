---
title: SharePoint- tai OneDrive-hallintakeskusta ei voi käyttää
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: 7ba4a9c6995c03dd21e0e1aa387e407d41a08fb1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824432"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>SharePoint- tai OneDrive-hallintakeskusta ei voi käyttää

- Jos SharePoint- tai OneDrive-hallintakeskussivustosi ei ole käytettävissä tai se ei ole käytettävissä, voi olla tilapäinen palveluongelma, jossa käyttäjillä voi olla ajoittaisia viiveitä tai siirtymisvirheitä SharePoint-sivustojen tai OneDrive-sisällön käytön aikana. Tarkista Palvelun [kunto -koontinäytöstä,](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) vaikuttaako se organisaatioosi.

- Yleisille ja SharePoint-järjestelmänvalvojille on oltava määritetty SharePoint-käyttöoikeus. Juuri luoduilla tileillä, jotka on juuri määritetty SharePoint-käyttöoikeus- tai järjestelmänvalvojan roolilla, voi i ie iä sharePointia käyttää, kuten "käyttö estetty" tai "käyttäjää ei löydy". Anna vähintään 24 tuntia aikaa suorittaa synkronointi eri järjestelmissä. Ymmärrämme, että 24 tuntia voi vaikuttaa pitkältä ajasta. Monissa tapauksissa ongelmaan on jo tehty ratkaisu.

- Privileged Identity Management[(PIM)](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)-käyttäjät voivat saada käyttö estettyjä tietoja, jos käyttöaikaikkuna on hyvin pieni, katso [Pim-tilien käyttö estetty.](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)