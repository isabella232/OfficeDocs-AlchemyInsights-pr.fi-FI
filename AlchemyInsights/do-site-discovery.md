---
title: Sivuston etsiminen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693489"
---
# <a name="do-site-discovery"></a>Sivuston etsiminen

Jos organisaatiosi käyttää edelleen vanhoja verkkosovelluksia ja aikoo käyttää Internet Explorer -tilaa (jota useimmat asiakkaat käyttävät), sinun kannattaa tehdä lisää sivuston etsintää.

**Olet jo ottanut käyttöön Vanhemman Microsoft Edge -version**

Jos olet jo määrittänyt yrityssivustoluettelon toimimaan Microsoft Edgen vanhan version kanssa, sivuston etsintä on melkein valmis. Yksi asia, joka sinun on ehkä lisättävä, on lisätä neutraalit sivustot.

Neutraalit sivustot ovat yleensä sivustoja, jotka tarjoavat kertakirjautumisen. Jos siirryt Microsoft Edgestä neutraaliin sivustoon, haluat pysyä Microsoft Edgessä todennetuksi. Jos siirryt neutraaliin sivustoon Internet Explorer -tilassa, haluat pysyä Internet Explorer -tilassa todentaaksesi sen.

Tunnista kaikki SSO-sivustot tai muut neutraalit sivustot, joita käytät, ja lisää ne yrityssivustoluetteloon.

**Internet Explorer on oletusselaimesi**

Jos käytät vain Internet Exploreria nyt, et ehkä tiedä, mitkä sivustot ovat päivitetneet moderneihin verkkostandardeihin ja mitkä edellyttävät edelleen Internet Exploreria. Haluat etsiä ja lisätä nämä sivustot yrityssivustoluetteloon, jotta voit käyttää Internet Explorer -tilaa vain kyseisissä sivustoissa.

> [!NOTE]
> [Enterprise Site Discovery löytää](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) sivustot, jotka saattavat tarvita Internet Explorer -tilaa. Se voi kerätä tietoja tietokoneista, joissa on Windows Internet Explorer 8 – Internet Explorer 11 Windows 10:ssä, Windows 8.1:ssä tai Windows 7:ssä.

**Tietojen analysointi**

Kun olet kerännyt sivustotiedot, suosittelemme tietojen analysoimiseen seuraavaa nelivaiheista prosessia:
1. Lajittele tiedot toimialueen ja URL-osoitteen mukaan.
2. Määritä internet Explorer -tilaa varten määritettävät sovelluksen rajat. Haluat sisällyttää kaikki sovelluksen määrittävät sivustot ja verkko-ohjausobjektit, mutta et halua sisällyttää ylimääräisiä sivustoja ja ohjausobjekteja. Jotkin sivustot voivat olla yhtä *https://contoso.com/app1* yksinkertaisia, kun taas toiset saattavat edellyttää useiden sivustojen ja sivujen määrittelemiseen.
3. Testaa sovellus sen varmistamiseksi, että se ei toimi natiivisti. Monet sivustot tarjoavat modernia sisältöä, kun ne tunnistavat nykyaikaisen selaimen ja tarjoavat vanhaa sisältöä vain, kun ne tunnistavat Internet Explorerin.
4. Lisää sovellus yrityssivustoluetteloon, jos sovelluksen testaus epäonnistuu.

> [!NOTE]
> Parhaana käytäntönä voit ryhmitellä kaikki sivustot, jotka muodostavat sovelluksen. Näin kun päivität sovelluksen, koko sivusto on helpompi poistaa Internet Explorer -tilasta ja aloittaa sovelluksen modernin selaimen käyttö.

Kun olet tehnyt sivuston etsinnän ja analysoinut tiedot, voit aloittaa kanavastrategian tarkastelemisen.

