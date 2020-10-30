---
title: Intune Exchangen paikallinen yhdistin
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: fi-FI
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807650"
---
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchangen paikallinen yhdistin

Jos haluat lisä tietoja yhdistimen määrittämisestä Intune-toiminnon ja paikallisen Exchange-sovelluksen välillä, tutustu seuraaviin ohje isiin:

[Paikallisen Exchange-yhdistimen määrittäminen Intunella Microsoft Intune Azure-sovelluksessa](https://docs.microsoft.com/intune/exchange-connector-install)

**USEIN kysytyt kysymykset**

K: näyttöön tulee virhe, kuten "Exchange Connector-versiota ei voi käyttää", kun yrität määrittää Exchange Connectoria. Mikä voi olla syynä?

A: käyttämäsi tilin käyttö oikeus on oikein-sillä on oltava aktiivinen Intune-käyttö oikeus

K: Onko mahdollista käyttää useita Exchange-yhdistimiä?

A: voit määrittää vain yhden Exchange Connector/Intune-vuokra ajan Exchange-organisaatiota kohden. Yhdistin voidaan asentaa vain yhteen palvelimeen usean palvelimen Exchange-organisaatiossa.

Et voi myöskään määrittää samassa vuokra ajassa määritettyä sekä Exchange Onlinea että Exchange Onlinen yhdistimiä.

K: Voiko yhdistin käyttää CAS-matriisia Exchangen yhteydessä?

A: CAS-matriisin määrittäminen ei ole yhteensopiva kokoonpano yhdistimen määrityksessä. Vain yksittäinen palvelin pitäisi määrittää, ja sen pitäisi olla kovakoodattu yhdistimen määritys tiedostossa, joka löytyy

ohjelmadata\microsoft\microsoft Intunen paikallinen Exchange Connector \ OnpremiseExchangeConnectorServiceConfiguration.xml

Etsi seuraava merkintä ```<ExchangeWebServiceURL />``` ja Vaihda URL-osoite Exchange-palvelimeen.

**Esimerkiksi**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Lisä tietoja vian määrityksestä on seuraavissa ohjeissa: [Intune-paikallisen Exchange Connectorin vian määritys](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Selväkielisen kirjaamisen ottaminen käyttöön Exchange Connectorissa**

1. Avaa Exchange Connector-jäljityksen määritys tiedosto muokkaamista varten.  
Tiedosto sijaitsee osoitteessa:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**Esimerkiksi**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Etsi TraceSourceLine seuraavalla avaimella: opremisesexchangecontactorservice  
  
3. SourceLevel-solmun arvon muuttaminen tietojen activerttracing (oletus)-kentän arvoksi verbose-pikatoimintojen jäljitys  

**Esimerkiksi**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. Microsoft Intune Exchange-palvelun käynnistäminen uudelleen  
5. Täysi synkronointi Intune-portaalissa, kunnes se on valmis, ja muuta sitten XML takaisin "Information Activitystracing" ja Käynnistä Microsoft Intune Exchange-palvelu uudelleen.  
6. Lokien sijainti on: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`