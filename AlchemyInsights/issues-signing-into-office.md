---
title: Kirjautumisongelmat Microsoft 365 sovelluksissa
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: f8f2824cc4a575ab7d7c9adec5b75e5955ec9fb5
ms.sourcegitcommit: b6dd6ae628a02ea6b997a993c49de083465bc2ac
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/30/2021
ms.locfileid: "58744633"
---
# <a name="issues-signing-into-microsoft-365-apps"></a>Kirjautumisongelmat Microsoft 365 -sovellukset

Huomautus: Jos käytät Windows:n vanhempaa versiota (esimerkiksi Windows 7 SP1- tai Windows Server 2008 R2 [](https://download.microsoft.com/download/0/6/5/0658B1A7-6D2E-474F-BC2C-D69E5B9E9A68/MicrosoftEasyFix51044.msi) -versiota), ota TLS 1.2 käyttöön oletusarvoisesti helpon korjauksen avulla. Lisätietoja on päivityksessä [TLS 1.1: n ja TLS 1.2:n ottaminen](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)käyttöön WinHTTP in Windows :n oletusarvoisen suojatun protokollan avulla.

Kokeile korjata Microsoft 365 -sovellusten kirjautumisongelmat seuraavien vaihtoehtojen avulla laitteessa, jossa ongelma ilmenee:  

- Lisätietoja Windows on [Suositukset yleisimmät kirjautumisongelmat.](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)
- Mac-tietokoneissa katso Office 2016 for Mac [kirjautuminen ei](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)

**Vihje** Voimme diagnosoida ja korjata useita Windows-tietokoneiden Officen yleisiä sisäänkirjautumisongelmia puolestasi automaattisesti. Jos haluat käyttää automaattista työkaluamme, lataa ja suorita **[Microsoftin tuki- ja palautusavustaja](https://aka.ms/SaRA-OfficeSignInScenario)**.

**Huomautus:** Modernin varmennuksen (ADAL) tai WWW-tilin hallinnan (KÄYTTÖOIKEUKSIEN) käytöstä poistaminen kirjautumis- tai **aktivointiongelmiin ei ole suositeltavaa.** Jos virheitä ilmenee yhdistettäessä Microsoft 365 Office 2013:n avulla, [](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) varmista, että otat modernin todennuksen käyttöön Office asiakasohjelmassa.

Lisätietoja vianmäärityksestä on kohdassa:

[Yhteysongelmat kirjautumisen yhteydessä Office 2016:n koontiversioon 16.0.7967 Windows 10:ssä](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[Et voi kirjautua organisaatiotiliisi, kuten Office 365, Azureen tai Intuneen](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[Muiden kuin selainsovellusten vianmääritys, jotka eivät voi kirjautua Office 365, Azureen tai Intuneen](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[Tunnistetietoja pyydetään toistuvasti Office](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)