---
title: Hallintakeskuksen SharePoint tai OneDrive käyttö ei onnistu
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
ms.openlocfilehash: afb28ccae2c9f087f1e1417cb6594cedc908e1cf759a5d1e6d92c4ee9a75527d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020441"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>Hallintakeskuksen SharePoint tai OneDrive käyttö ei onnistu

- Jos SharePoint- tai OneDrive-hallintakeskussivustosi ei ole käytettävissä tai se ei ole käytettävissä, voi olla tilapäinen palveluongelma, jossa käyttäjillä ilmenee ajoittain viiveitä tai siirtymisvirheitä, kun he SharePoint sivustoja tai OneDrive sisältöä. Tarkista Palvelun [kunto -koontinäytöstä,](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) vaikuttaako se organisaatioosi.

- Yleiset ja SharePoint järjestelmänvalvojille on oltava määritettynä SharePoint käyttöoikeus. Juuri luoduilla tileillä, jotka on juuri määritetty SharePoint käyttöoikeus- tai järjestelmänvalvojan roolilla, voi i ie i iä SharePoint käyttöongelmia, kuten "käyttö estetty" tai "käyttäjää ei löydy". Anna vähintään 24 tuntia aikaa suorittaa synkronointi eri järjestelmissä. Ymmärrämme, että 24 tuntia voi vaikuttaa pitkältä ajasta. Monissa tapauksissa ongelmaan on jo tehty ratkaisu.

- Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) käyttäjät voivat saada käyttö estetty, jos sallittu käyttöaika on erittäin pieni, katso [Kohta PIM-tilien](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)käyttö estetty.