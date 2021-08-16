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
ms.openlocfilehash: 4653fdef7e9226f05809d56e9a445cd1da35b0578c088bea72252a281d4527d2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: fi-FI
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030755"
---
# <a name="do-site-discovery"></a>Sivuston etsiminen

Jos organisaatiossasi käytetään edelleen vanhoja verkkosovelluksia ja suunnittelee käyttävänsä Internet Explorer -tilaa (jota useimmat asiakkaat käyttävät), sinun kannattaa tehdä lisää sivuston etsintää.

**Olet jo ottanut käyttöön vanhemman Microsoft Edge**

Jos olet jo määrittänyt yrityssivustoluettelon toimimaan vanhan Microsoft Edge, sivuston etsintä on melkein valmis. Yksi asia, joka sinun on ehkä lisättävä, on lisätä neutraalit sivustot.

Neutraalit sivustot ovat yleensä sivustoja, joissa on kertakirjautuminen. Jos siirryt neutraalille sivustolle Microsoft Edge, haluat pysyä Microsoft Edge todentaa. Jos siirryt neutraaliin sivustoon Internet Explorer -tilassa, haluat pysyä Internet Explorer -tilassa todentaaksesi sen.

Tunnista mahdolliset SSO-ruudut tai muut neutraalit sivustot, joita käytät, ja lisää ne yrityssivustoluetteloosi.

**Internet Explorer on oletusselaimesi**

Jos käytät vain Internet Exploreria nyt, et ehkä tiedä, mitkä sivustot ovat päivittäneet moderneihin verkkostandardeihin ja mitkä edellyttävät edelleen Internet Exploreria. Haluat etsiä ja lisätä nämä sivustot yrityssivustoluetteloon, jotta voit käyttää vain kyseisissä sivustoissa Internet Explorer -tilaa.

> [!NOTE]
> [Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) löytää sivustot, jotka saattavat tarvita Internet Explorer -tilaa. Se voi kerätä tietoja tietokoneissa, joissa Windows Internet Explorer 8 – Internet Explorer 11 Windows 10, Windows 8.1 tai Windows 7.

**Analysoi tiedot**

Kun olet kerännyt sivustotiedot, suosittelemme tietojen analysointiin seuraavaa nelivaiheista prosessia:
1. Lajittele tiedot toimialueen ja URL-osoitteen mukaan.
2. Määritä Internet Explorer -tilaa varten määritettävät sovelluksen rajat. Haluat sisällyttää kaikki sovelluksen määrittävät sivustot ja verkko-ohjausobjektit, mutta et halua sisällyttää lisäsivustoja ja -ohjausobjekteja. Jotkin sivustot voivat olla yhtä *https://contoso.com/app1* yksinkertaisia, kun taas toiset saattavat edellyttää useiden sivustojen ja sivujen määrittelemiseen.
3. Testaa sovellus sen varmistamiseksi, että se ei toimi natiivisti. Monet sivustot tarjoavat modernia sisältöä, kun ne tunnistavat nykyaikaisen selaimen ja tarjoavat vanhaa sisältöä vain Internet Exploreria tunnistaessaan.
4. Lisää sovellus Yrityssivustoluetteloon, jos sovelluksen testaus epäonnistuu.

> [!NOTE]
> Paras käytäntö on ryhmitellä kaikki sivustot, jotka muodostavat sovelluksen. Kun päivität sovelluksen, koko sivusto on helpompi poistaa Internet Explorer -tilasta ja sovelluksen modernia selainta on helpompi käyttää.

Kun olet tehnyt sivuston etsinnän ja analysoinut tiedot, voit aloittaa kanavastrategian tarkastelemisen.

