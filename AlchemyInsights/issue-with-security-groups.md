---
title: Ongelma käyttöoikeusryhmissä
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
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177493"
---
# <a name="issue-with-security-groups"></a>Ongelma käyttöoikeusryhmissä

**Jos saat verkkovirheen AADDS104**

Virheelliset verkon käyttöoikeusryhmän säännöt ovat yleisin azure Active Directory -toimialueen palveluiden (AD DS) verkkovirheiden syy. Virtuaalisen verkon käyttöoikeusryhmän on sallittava tiettyjen porttien ja protokollien käyttö. Jos nämä portit on estetty, Azure-ympäristö ei voi valvoa tai päivittää hallittua toimialuetta. Tämä vaikuttaa myös Azure AD:n ja Azure AD DS:n väliseen synkronointiin. Varmista, että oletusportit ovat avoinna, jotta palvelu ei keskeydy.

Lisätietoja yleisistä verkon käyttöoikeusryhmän määritysongelmista ja niiden ratkaisemisesta on kohdassa Käyttöoikeusryhmien lisääminen [ja tarkistaminen.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)
